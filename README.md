# cgr -- change registry | yarn & npm registry manager

`cgr` can help you easy and fast switch between different npm or yarn registries,
now include: `npm`, `cnpm`, `taobao`, `nj(nodejitsu)`, `rednpm`.

## Install

```
$ npm install -g cgr
```

## Example

npm registry is the same as yarn registry

```
$ cgr ls

  npm -----  https://registry.npmjs.org/
  cnpm ----  http://r.cnpmjs.org/
* taobao --  https://registry.npm.taobao.org/
  nj ------  https://registry.nodejitsu.com/
  rednpm -- http://registry.mirror.cqupt.edu.cn
  skimdb -- https://skimdb.npmjs.com/registry

```

npm registry is different from yarn registry

```
$ cgr ls

N npm -----  https://registry.npmjs.org/
  cnpm ----  http://r.cnpmjs.org/
Y taobao --  https://registry.npm.taobao.org/
  nj ------  https://registry.nodejitsu.com/
  rednpm -- http://registry.mirror.cqupt.edu.cn
  skimdb -- https://skimdb.npmjs.com/registry

```

```
$ cgr use cnpm  //switch registry to cnpm

    npm Registry has been set to: http://r.cnpmjs.org/
    yarn Registry has been set to: http://r.cnpmjs.org/

```

```
$ cgr use cnpm y  //switch registry to cnpm

    yarn Registry has been set to: http://r.cnpmjs.org/

```

## Usage

```
Usage: cgr [options] [command]

  Commands:

    ls                           List all the registries
    use <registry> [type]        Change registry to registry
    add <registry> <url> [home]  Add one custom registry
    del <registry>               Delete one custom registry
    test [registry]              Show the response time for one or all registries
    help                         Print this help

  Options:

    -h, --help     output usage information
    -V, --version  output the version number
```

## Registries

- [npm](https://www.npmjs.org)
- [cnpm](http://cnpmjs.org)
- [nodejitsu](https://www.nodejitsu.com)
- [taobao](http://npm.taobao.org/)
- [rednpm](http://npm.mirror.cqupt.edu.cn)

## Notice

When you use an other registry, you can not use the `publish` command.

## LICENSE

MIT
