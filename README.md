# codeclimate-types

[![github actions](https://github.com/remcohaszing/codeclimate-types/actions/workflows/ci.yaml/badge.svg)](https://github.com/remcohaszing/codeclimate-types/actions/workflows/ci.yaml)
[![npm version](https://img.shields.io/npm/v/codeclimate-types)](https://www.npmjs.com/package/codeclimate-types)
[![npm downloads](https://img.shields.io/npm/dm/codeclimate-types)](https://www.npmjs.com/package/codeclimate-types)

TypeScript type definitions for
[Code Climate reports](https://github.com/codeclimate/platform/blob/master/spec/analyzers/SPEC.md)

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Related Projects](#related-projects)
- [License](#license)

## Installation

```sh
npm install codeclimate-types
```

## Usage

This package can be used to work with
[Code Climate reports](https://github.com/codeclimate/platform/blob/master/spec/analyzers/SPEC.md#issues)
in a type-safe manner. A practical use case is to generate a
[GitLab code quality](https://docs.gitlab.com/ee/ci/testing/code_quality.html) artifact.

## API

The package exports the following types:

- `Issue` — An issue represents a single instance of a real or potential code problem, detected by a
  static analysis Engine.
- `Category` — Issues must be associated with one or more categories.
- `Location` — Locations refer to ranges of a source code file.
- `Position` — Positions refer to specific characters within a source file.
- `Content` — Content gives more information about the issue’s check.
- `Trace` — Some engines require the ability to refer to other source locations in describing an
  issue.
- `Severity` — A severity string describing the potential impact of the issue found.

## Related Projects

- [`eslint-formatter-gitlab`](https://gitlab.com/remcohaszing/eslint-formatter-gitlab) — Show ESLint
  results directly in the GitLab code quality results

## License

[MIT](LICENSE.md) © [Remco Haszing](https://github.com/remcohaszing)
