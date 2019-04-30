[![Build Status](https://travis-ci.org/kaelzhang/generator-es-cross.svg?branch=master)](https://travis-ci.org/kaelzhang/generator-es-cross)
<!-- [![Coverage](https://codecov.io/gh/kaelzhang/generator-es-cross/branch/master/graph/badge.svg)](https://codecov.io/gh/kaelzhang/generator-es-cross) -->
<!-- optional appveyor tst
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/github/kaelzhang/generator-es-cross?branch=master&svg=true)](https://ci.appveyor.com/project/kaelzhang/generator-es-cross)
-->
<!-- optional npm version
[![NPM version](https://badge.fury.io/js/generator-es-cross.svg)](http://badge.fury.io/js/generator-es-cross)
-->
<!-- optional npm downloads
[![npm module downloads per month](http://img.shields.io/npm/dm/generator-es-cross.svg)](https://www.npmjs.org/package/generator-es-cross)
-->
<!-- optional dependency status
[![Dependency Status](https://david-dm.org/kaelzhang/generator-es-cross.svg)](https://david-dm.org/kaelzhang/generator-es-cross)
-->

# generator-es-cross

Yeoman generator to create a nodejs library to support both esm and commonjs by using `package.main` and `package.module`

## Install

```sh
$ npm i -g generator-es-cross
```

## Usage

```sh
# It is recommanded to clone the empty repo first,
# `generator-es-cross` reads the git remote url
#   and set default prompts values.
git clone git@github.com:my-name/my-empty-repo.git

cd my-empty-repo

yo es-cross
```

After that

- ES module files will be located at `./src`
- ES modules will be transformed into commonjs to directory `./lib` which is ignored by git.
- `package.main` -> `./lib`
- `package.module` -> `./src`
- both directory `src` and directory `lib` will be included in NPM tarball.

## License

[MIT](LICENSE)
