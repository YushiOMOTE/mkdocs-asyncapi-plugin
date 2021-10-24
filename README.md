# Mkdocs Async API Plugin

[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PyPi](https://img.shields.io/pypi/v/mkdocs-asyncapi-plugin.svg)](https://pypi.python.org/pypi/mkdocs-asyncapi-plugin)
[![Supported python versions](https://img.shields.io/pypi/pyversions/mkdocs-asyncapi-plugin.svg)](https://pypi.org/project/mkdocs-asyncapi-plugin/)

## Setup

1. Install [`asyncapi/generator`](https://github.com/asyncapi/generator)

``` sh
npm install -g @asyncapi/generator
```

2. Install this plugin.

``` sh
pip install mkdocs-asyncapi-plugin
```

3. Add `render_asyncapi` to `mkdocs.yml`:

``` yaml
plugins:
  - render_asyncapi
```

## Usage

Create a new markdown file which contains only this line:

``` markdown
!!asyncapi <path-to-spec-file>!!
```

`path-to-spec-file` is the path to the AsyncAPI spec file relative to the root of the repository (where you run `mkdocs`).

Then, the entire content of this file will be the AsyncAPI spec.
