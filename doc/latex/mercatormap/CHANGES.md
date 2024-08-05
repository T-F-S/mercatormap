# Changelog
All notable changes to this project will be documented in this file.

The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to
[Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
### Changed
### Deprecated
### Removed
### Fixed
### Security



## [1.2.0] - 2024-08-05

### Added
- Command `\ifmrcNPexists` to test existence of a named position
- Macros `\mrcAnimAngle` and `\l_mermap_anim_angle_fp` to measure
    the current orthodrome angle
- Animation example for static maps    

### Changed
- `\mrcNPlat` and `\mrcNPlon` result to 0 now, if named position does not exist
- `\ifmrcNPinmap` and `\ifmrcNPinvicinity` result to `false` now, if named position does not exist
- Point definitions on an orthodrome now take an optional angle as result:
    - Command `mrcNPfromOrthoFraction`
    - Command `mrcNPfromOrthoFractionNamed`
    - Command `mrcNPfromOrthoDistance`
    - Command `mrcNPfromOrthoDistanceNamed`

### Fixed
- Documentation contained dates from `2023` instead of `2024`



## [1.1.0] - 2024-08-01

### Added
- New supply sources (web tile servers):
    - `thunderforest atlas`
    - `topplusopen web light`
    - `topplusopen web light grau`
- Needed LaTeX version 2023-11-01
- Point definitions on an orthodrome:
    - Command `mrcNPfromOrthoFraction`
    - Command `mrcNPfromOrthoFractionNamed`
    - Command `mrcNPfromOrthoDistance`
    - Command `mrcNPfromOrthoDistanceNamed`
- Animation support:
    - Environment `mrcAnimation`
    - Command `\mrcTimewarpIdentity`
    - Command `\mrcTimewarpSlowStart`
    - Command `\mrcTimewarpSlowFinal`
    - Command `\mrcTimewarpSlowStartFinal`
    - Command `\mrcAnimFrame`
    - Command `\l_mermap_anim_frame_int`
    - Command `\mrcAnimTime`
    - Command `\l_mermap_anim_time_fp`
    - Command `\mrcAnimScaleDenom`
    - Command `\l_mermap_anim_scaledenom_fp`
    - Command `\mrcAnimLatitude`
    - Command `\l_mermap_anim_lat_fp`
    - Command `\mrcAnimLongitude`
    - Command `\l_mermap_anim_lon_fp`
    - Option `start-position`
    - Option `named-start-position`
    - Option `final-position`
    - Option `named-final-position`
    - Option `position`
    - Option `named-position`
    - Option `frames`
    - Option `drop-first-frame`
    - Option `drop-last-frame`
    - Option `drop-no-frame`
    - Option `scale-denominators`
    - Option `common-scale-denominator`
    - Option `timewarp`
    - Option `timewarp-identity`
    - Option `timewarp-slow-start`
    - Option `timewarp-slow-final`
    - Option `timewarp-slow-start-final`

### Changed
- Version history moved from documentation Chapter 11 to this changelog
- Versioning changed to [Semantic Versioning](http://semver.org/spec/v2.0.0.html)
    starting with 1.1.0
- `README` changed to `README.md`
- Key names start with `mermap` instead of `/mermap` now
- All common scratch variables like `\l_tmpa_tl` replaced by package variables
- Orthodrome code
- Several code further revisions

### Deprecated
- Stamen Design has discontinued to server map tiles since 2023-07-31.
    Therefore, all `supply/source` options based on Stamen Design are
    deprecated now, namely
    - `stamen terrain`
    - `stamen terrain-background`
    - `stamen terrain-labels`
    - `stamen terrain-lines`
    - `stamen toner`
    - `stamen toner-lite`
    - `stamen toner-hybrid`
    - `stamen toner-background`
    - `stamen toner-labels`
    - `stamen toner-lines`
    - `stamen watercolor`
    All these options are now not documented any more, but for some time
    are still available for old documents with cached map tiles.

### Removed
- Requirement for packages `expl3`, `xparse`, and `pdftexcmds`

### Fixed
- Links to the WMS maps of Bundesamt für Kartographie und Geodäsie changed
- Overwrite warning while generating `maptiles.texpy`
- Orthodrome drawing with identical starting and final point is now silently ignored



## [1.02] - 2020-08-06

### Added
- New options
  `/mermap/supply/area from marker input` and
  `/mermap/supply/add area from marker input`
  which allow to fit a map to a given external list of marker positions.
- New option `/mermap/fail on missing resource` to control
  compilation behavior for missing resource files.
- New marker option `/mermap/marker/distance` with corresponding
  macro `\mrcmarkerdistance` (issue #2)

### Deprecated
- Openrouteservice has discontinued mapsurfer tiles since June 2020.
  Therefore, `/mermap/supply/source=openrouteservice mapsurfer`
  is deprecated now. It is not documented any more, but
  for some time it is still available for old documents with
  cached map tiles.



## [1.01] - 2020-05-05

### Added
- New general marker option
  `/mermap/marker/generic` with corresponding macros
  `\mrcmarkergeneric` and `\l_mermap_marker_generic_tl`.
  Also, the marker uuid is made expl3 accessible as `\l_mermap_marker_uuid_tl`.
- New hyper marker options:
    - `/mermap/marker/url`
    - `/mermap/marker/link`
    - `/mermap/marker/use urls`
    - `/mermap/marker/ignore urls`
    - `/mermap/marker/use links`
    - `/mermap/marker/ignore links`

### Changed
- User messages for failed Python script calls are changed from warnings to
  errors to fail fast and to provide more information and hints about
  possible reasons.

### Fixed
- Sorting of index key entries fixed for the documentation.



## [1.00] - 2020-04-20

### Added
- Initial public release
