# Release notes

## v0.7.8 - 2015-10-22

### Fix

* Better error messages in case of HTTP-errors.

## v0.7.7 - 2015-10-19

### Fix

* Update dependencies
* Add `files`-property to package.json
* Input of "getPromise" must JSON-parsed (Fixes loading swagger-specs via HTTP)

## v0.7.6 - 2015-10-17
### Fix

* Issue #7: ReferenceError: httpGet is not defined 
  

## v0.7.4, v0.7.5 - 2015-10-15
### Change

* Bootprint now uses `customize` and its engines. This is only an internal change
  and should not affect the API or the configuration. It allows for more flexibility 
  in the future.

## v0.7.3 - 2015-09-03
### Fixed

- When passing a plaing object as data, bootprint has thrown an exception 

## v0.7.2 - 2015-09-01
### Fixed

- Development-Mode did not start watcher on Handlebars partials

## v0.7.1 - 2015-07-20
### Fixed

- Compatibility code fixed...


## v0.7.0 - 2015-07-20
### Fixed

- Compatibility code for legaxy config format did not respect all possible variations.

## v0.6.0 - 2015-07-20
### Changed

- Template configuration should now be done with `options.handlebars.templates` pointing to a directory
  containing a `index.html.hbs` file (instead of using `options.handlebars.template` to point to a
  template file). Old behaviour still supported. Multiple template files might be supported in the future.
- Pre-processor configuration should now be done with `options.handlebars.preprocessor`

## v0.5.1 - 2015-06-22
### Fixed
- Fix to support legacy config format.
  This was broken in 0.5.0  

## v0.5.0 - 2015-06-22
### Changed

- Preferred path for handlebars options is now in `options.handlebars` (instead of `options`)
  with old configuration still supported
- Support for specifiying a target-filename in `options.handlebars.targetFile` (defaults to `index.html`)


## v0.4.12 - 2015-06-21
### Fixed

- Remove `request` from dependencies

## v0.4.11 - 2015-06-20
### Fixed

- Reduces total extracted size of bootprint by 9 MB, by replacing `request` by `get-promise`
- Display uncaught exceptions with proper stack-traces

## v0.4.10 - 2015-06-18
### Added

- Output used template-module versions

## v0.4.9 - 2015-06-17
### Fixed                          

- `Cannot read property 'bind' of undefined` occuring when running a template-module with preprocessor

## 0.4.7 (2015-04-07)

### Added 

- Handlebars helpers can be registered by a path to a JavaScript-file, instead of directly
    calling "require" with the file.
- &lt;spec> in command-line-interface can also be path to a template-module

## v0.4.6 (2015-04-07)

### Fixed

- [#1: cli.js not found when installing from npm or master](https://github.com/nknapp/bootprint/issues/1)

