# JavaScript + TypeScript Target Runtime for ANTLR 4

[![Build & Test](https://github.com/mike-lischke/antlr4ng/actions/workflows/nodejs.yml/badge.svg?branch=master)](https://github.com/mike-lischke/antlr4ng/actions/workflows/nodejs.yml)
[![Downloads](https://img.shields.io/npm/dw/antlr4ng?color=blue)](https://www.npmjs.com/package/antlr4ng)
[![npm version](https://img.shields.io/npm/v/antlr4ng?color=yellow)](https://www.npmjs.com/package/antlr4ng)


This package is a fork of the official ANTLR4 JavaScript runtime, with the following changes:

- Much improved TypeScript type definitions.
- XPath implementation.
- Vocabulary implementation.
- Complete Interval implementation.
- Consistent formatting (indentation, semicolons, spaces, etc.).
- Numerous smaller fixes (`null` instead of `undefined` and others).
- Smaller node package (no test specs or other unnecessary files).

It is a drop-in replacement of the `antlr4` package, and can be used as such. For more information about ANTLR see www.antlr.org. More details about the JavaScript/TypeScript target can be found [here](https://github.com/antlr/antlr4/blob/master/doc/javascript-target.md).

## Release Notes

### 1.0.2
- Github build action
- Updated package.json
- Exported `ErrorNode`

### 1.0.1

- Added and/or replaced all copyrights to a common ANTLR version.
- Removed all individual default exports. Only the final lib exports contain both, default and non-default exports. This avoids namespace access like `antlr4.atn`. Everything is available under a top level import.
- Renamed ErrorListener to BaseListener, as that is what it is actually when comparing it to the Java runtime.

### 1.0.0

- Initial release.
