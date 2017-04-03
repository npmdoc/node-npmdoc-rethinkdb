# api documentation for  [rethinkdb (v2.3.3)](http://rethinkdb.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-rethinkdb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rethinkdb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rethinkdb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rethinkdb)
#### This package provides the JavaScript driver library for the RethinkDB database server for use in your node application.

[![NPM](https://nodei.co/npm/rethinkdb.png?downloads=true)](https://www.npmjs.com/package/rethinkdb)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rethinkdb/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-rethinkdb_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rethinkdb/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rethinkdb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rethinkdb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "http://github.com/rethinkdb/rethinkdb/issues",
        "email": "bugs@rethinkdb.com"
    },
    "dependencies": {
        "bluebird": ">= 2.3.2 < 3"
    },
    "description": "This package provides the JavaScript driver library for the RethinkDB database server for use in your node application.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "3dc6586e22fa1dabee0d254e64bd0e379fad2f72",
        "tarball": "https://registry.npmjs.org/rethinkdb/-/rethinkdb-2.3.3.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "files": [
        "rethinkdb.js",
        "ast.js",
        "net.js",
        "util.js",
        "errors.js",
        "cursor.js",
        "README.md",
        "proto-def.js"
    ],
    "homepage": "http://rethinkdb.com",
    "keywords": [
        "database",
        "NoSQL",
        "reql",
        "query language"
    ],
    "main": "rethinkdb",
    "maintainers": [
        {
            "name": "rethinkdb",
            "email": "bugs@rethinkdb.com"
        }
    ],
    "name": "rethinkdb",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/rethinkdb/rethinkdb.git"
    },
    "scripts": {},
    "version": "2.3.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module rethinkdb](#apidoc.module.rethinkdb)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>Error.RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>ISO8601 ()](#apidoc.element.rethinkdb.ISO8601)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird (resolver)](#apidoc.element.rethinkdb._bluebird)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird._SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>add ()](#apidoc.element.rethinkdb.add)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>and ()](#apidoc.element.rethinkdb.and)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>april {{signature}}](#apidoc.element.rethinkdb.april)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>args ()](#apidoc.element.rethinkdb.args)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>asc ()](#apidoc.element.rethinkdb.asc)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>august {{signature}}](#apidoc.element.rethinkdb.august)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>avg ()](#apidoc.element.rethinkdb.avg)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>binary ()](#apidoc.element.rethinkdb.binary)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>branch ()](#apidoc.element.rethinkdb.branch)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>ceil ()](#apidoc.element.rethinkdb.ceil)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>circle ()](#apidoc.element.rethinkdb.circle)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>connect ()](#apidoc.element.rethinkdb.connect)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>contains ()](#apidoc.element.rethinkdb.contains)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>count ()](#apidoc.element.rethinkdb.count)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>db ()](#apidoc.element.rethinkdb.db)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>dbCreate ()](#apidoc.element.rethinkdb.dbCreate)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>dbDrop ()](#apidoc.element.rethinkdb.dbDrop)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>dbList ()](#apidoc.element.rethinkdb.dbList)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>december {{signature}}](#apidoc.element.rethinkdb.december)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>desc ()](#apidoc.element.rethinkdb.desc)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>distance ()](#apidoc.element.rethinkdb.distance)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>distinct ()](#apidoc.element.rethinkdb.distinct)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>div ()](#apidoc.element.rethinkdb.div)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>do ()](#apidoc.element.rethinkdb.do)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>epochTime ()](#apidoc.element.rethinkdb.epochTime)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>eq ()](#apidoc.element.rethinkdb.eq)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>error ()](#apidoc.element.rethinkdb.error)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>expr ()](#apidoc.element.rethinkdb.expr)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>february {{signature}}](#apidoc.element.rethinkdb.february)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>floor ()](#apidoc.element.rethinkdb.floor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>friday {{signature}}](#apidoc.element.rethinkdb.friday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>ge ()](#apidoc.element.rethinkdb.ge)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>geojson ()](#apidoc.element.rethinkdb.geojson)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>grant ()](#apidoc.element.rethinkdb.grant)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>group ()](#apidoc.element.rethinkdb.group)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>gt ()](#apidoc.element.rethinkdb.gt)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>http ()](#apidoc.element.rethinkdb.http)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>info ()](#apidoc.element.rethinkdb.info)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>intersects ()](#apidoc.element.rethinkdb.intersects)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>january {{signature}}](#apidoc.element.rethinkdb.january)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>js ()](#apidoc.element.rethinkdb.js)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>json ()](#apidoc.element.rethinkdb.json)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>july {{signature}}](#apidoc.element.rethinkdb.july)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>june {{signature}}](#apidoc.element.rethinkdb.june)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>le ()](#apidoc.element.rethinkdb.le)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>line ()](#apidoc.element.rethinkdb.line)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>literal ()](#apidoc.element.rethinkdb.literal)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>lt ()](#apidoc.element.rethinkdb.lt)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>map ()](#apidoc.element.rethinkdb.map)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>march {{signature}}](#apidoc.element.rethinkdb.march)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>max ()](#apidoc.element.rethinkdb.max)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>maxval {{signature}}](#apidoc.element.rethinkdb.maxval)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>may {{signature}}](#apidoc.element.rethinkdb.may)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>min ()](#apidoc.element.rethinkdb.min)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>minval {{signature}}](#apidoc.element.rethinkdb.minval)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>mod ()](#apidoc.element.rethinkdb.mod)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>monday {{signature}}](#apidoc.element.rethinkdb.monday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>mul ()](#apidoc.element.rethinkdb.mul)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>ne ()](#apidoc.element.rethinkdb.ne)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>net.Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>net.HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>net.TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>not ()](#apidoc.element.rethinkdb.not)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>november {{signature}}](#apidoc.element.rethinkdb.november)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>now ()](#apidoc.element.rethinkdb.now)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>object ()](#apidoc.element.rethinkdb.object)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>october {{signature}}](#apidoc.element.rethinkdb.october)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>or ()](#apidoc.element.rethinkdb.or)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>point ()](#apidoc.element.rethinkdb.point)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>polygon ()](#apidoc.element.rethinkdb.polygon)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>random ()](#apidoc.element.rethinkdb.random)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>range ()](#apidoc.element.rethinkdb.range)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>reduce ()](#apidoc.element.rethinkdb.reduce)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>round ()](#apidoc.element.rethinkdb.round)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>row {{signature}}](#apidoc.element.rethinkdb.row)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>saturday {{signature}}](#apidoc.element.rethinkdb.saturday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>september {{signature}}](#apidoc.element.rethinkdb.september)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>sub ()](#apidoc.element.rethinkdb.sub)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>sum ()](#apidoc.element.rethinkdb.sum)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>sunday {{signature}}](#apidoc.element.rethinkdb.sunday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>table ()](#apidoc.element.rethinkdb.table)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>tableCreate ()](#apidoc.element.rethinkdb.tableCreate)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>tableDrop ()](#apidoc.element.rethinkdb.tableDrop)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>tableList ()](#apidoc.element.rethinkdb.tableList)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>thursday {{signature}}](#apidoc.element.rethinkdb.thursday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>time ()](#apidoc.element.rethinkdb.time)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>tuesday {{signature}}](#apidoc.element.rethinkdb.tuesday)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>typeOf ()](#apidoc.element.rethinkdb.typeOf)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>union ()](#apidoc.element.rethinkdb.union)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>uuid ()](#apidoc.element.rethinkdb.uuid)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>wednesday {{signature}}](#apidoc.element.rethinkdb.wednesday)
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAuthError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAvailabilityError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlCompileError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlDriverCompileError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlInternalError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlNonExistenceError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpFailedError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpIndeterminateError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlPermissionError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlQueryLogicError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlResourceLimitError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlRuntimeError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlServerCompileError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlTimeoutError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlUserError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>Error.RqlClientError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.AggregateError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.CancellationError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.OperationalError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.PromiseInspection.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.TimeoutError.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird._SomePromiseArray.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>cursor
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>net
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>net.Connection.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>net.HttpConnection.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>net.TcpConnection.prototype
1.  object <span class="apidocSignatureSpan">rethinkdb.</span>util

#### [module rethinkdb.Error](#apidoc.module.rethinkdb.Error)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverError ()](#apidoc.element.rethinkdb.Error.ReqlDriverError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlCompileError ()](#apidoc.element.rethinkdb.Error.RqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlDriverError ()](#apidoc.element.rethinkdb.Error.RqlDriverError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlRuntimeError ()](#apidoc.element.rethinkdb.Error.RqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlServerError ()](#apidoc.element.rethinkdb.Error.RqlServerError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>printQuery (term)](#apidoc.element.rethinkdb.Error.printQuery)

#### [module rethinkdb.Error.ReqlAuthError](#apidoc.module.rethinkdb.Error.ReqlAuthError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.ReqlAuthError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.</span>__super__

#### [module rethinkdb.Error.ReqlAuthError.prototype](#apidoc.module.rethinkdb.Error.ReqlAuthError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.prototype.constructor)

#### [module rethinkdb.Error.ReqlAvailabilityError](#apidoc.module.rethinkdb.Error.ReqlAvailabilityError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.ReqlAvailabilityError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.</span>__super__

#### [module rethinkdb.Error.ReqlAvailabilityError.prototype](#apidoc.module.rethinkdb.Error.ReqlAvailabilityError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.prototype.constructor)

#### [module rethinkdb.Error.ReqlCompileError](#apidoc.module.rethinkdb.Error.ReqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.ReqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.</span>__super__

#### [module rethinkdb.Error.ReqlCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlCompileError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.prototype.constructor)

#### [module rethinkdb.Error.ReqlDriverCompileError](#apidoc.module.rethinkdb.Error.ReqlDriverCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.ReqlDriverCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.</span>__super__

#### [module rethinkdb.Error.ReqlDriverCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlDriverCompileError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.prototype.constructor)

#### [module rethinkdb.Error.ReqlError](#apidoc.module.rethinkdb.Error.ReqlError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError.ReqlError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.</span>__super__

#### [module rethinkdb.Error.ReqlError.prototype](#apidoc.module.rethinkdb.Error.ReqlError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.prototype.</span>constructor (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError.prototype.constructor)

#### [module rethinkdb.Error.ReqlInternalError](#apidoc.module.rethinkdb.Error.ReqlInternalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.ReqlInternalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.</span>__super__

#### [module rethinkdb.Error.ReqlInternalError.prototype](#apidoc.module.rethinkdb.Error.ReqlInternalError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.prototype.constructor)

#### [module rethinkdb.Error.ReqlNonExistenceError](#apidoc.module.rethinkdb.Error.ReqlNonExistenceError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.ReqlNonExistenceError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.</span>__super__

#### [module rethinkdb.Error.ReqlNonExistenceError.prototype](#apidoc.module.rethinkdb.Error.ReqlNonExistenceError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.prototype.constructor)

#### [module rethinkdb.Error.ReqlOpFailedError](#apidoc.module.rethinkdb.Error.ReqlOpFailedError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.ReqlOpFailedError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.</span>__super__

#### [module rethinkdb.Error.ReqlOpFailedError.prototype](#apidoc.module.rethinkdb.Error.ReqlOpFailedError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.prototype.constructor)

#### [module rethinkdb.Error.ReqlOpIndeterminateError](#apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.ReqlOpIndeterminateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.</span>__super__

#### [module rethinkdb.Error.ReqlOpIndeterminateError.prototype](#apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.prototype.constructor)

#### [module rethinkdb.Error.ReqlPermissionError](#apidoc.module.rethinkdb.Error.ReqlPermissionError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.ReqlPermissionError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.</span>__super__

#### [module rethinkdb.Error.ReqlPermissionError.prototype](#apidoc.module.rethinkdb.Error.ReqlPermissionError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.prototype.constructor)

#### [module rethinkdb.Error.ReqlQueryLogicError](#apidoc.module.rethinkdb.Error.ReqlQueryLogicError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.ReqlQueryLogicError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.</span>__super__

#### [module rethinkdb.Error.ReqlQueryLogicError.prototype](#apidoc.module.rethinkdb.Error.ReqlQueryLogicError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.prototype.constructor)

#### [module rethinkdb.Error.ReqlResourceLimitError](#apidoc.module.rethinkdb.Error.ReqlResourceLimitError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.ReqlResourceLimitError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.</span>__super__

#### [module rethinkdb.Error.ReqlResourceLimitError.prototype](#apidoc.module.rethinkdb.Error.ReqlResourceLimitError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.prototype.constructor)

#### [module rethinkdb.Error.ReqlRuntimeError](#apidoc.module.rethinkdb.Error.ReqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.ReqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.</span>__super__

#### [module rethinkdb.Error.ReqlRuntimeError.prototype](#apidoc.module.rethinkdb.Error.ReqlRuntimeError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.prototype.constructor)

#### [module rethinkdb.Error.ReqlServerCompileError](#apidoc.module.rethinkdb.Error.ReqlServerCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.ReqlServerCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.</span>__super__

#### [module rethinkdb.Error.ReqlServerCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlServerCompileError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.prototype.constructor)

#### [module rethinkdb.Error.ReqlTimeoutError](#apidoc.module.rethinkdb.Error.ReqlTimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.ReqlTimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.</span>__super__

#### [module rethinkdb.Error.ReqlTimeoutError.prototype](#apidoc.module.rethinkdb.Error.ReqlTimeoutError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.prototype.constructor)

#### [module rethinkdb.Error.ReqlUserError](#apidoc.module.rethinkdb.Error.ReqlUserError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError.ReqlUserError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlUserError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.</span>__super__

#### [module rethinkdb.Error.ReqlUserError.prototype](#apidoc.module.rethinkdb.Error.ReqlUserError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlUserError.prototype.constructor)

#### [module rethinkdb.Error.RqlClientError](#apidoc.module.rethinkdb.Error.RqlClientError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError.RqlClientError)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.RqlClientError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.</span>__super__

#### [module rethinkdb.Error.RqlClientError.prototype](#apidoc.module.rethinkdb.Error.RqlClientError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.RqlClientError.prototype.constructor)

#### [module rethinkdb._bluebird](#apidoc.module.rethinkdb._bluebird)
1.  [function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird (resolver)](#apidoc.element.rethinkdb._bluebird._bluebird)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>Promise (resolver)](#apidoc.element.rethinkdb._bluebird.Promise)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>RangeError ()](#apidoc.element.rethinkdb._bluebird.RangeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>RejectionError (message)](#apidoc.element.rethinkdb._bluebird.RejectionError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TypeError ()](#apidoc.element.rethinkdb._bluebird.TypeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>_SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>all (promises)](#apidoc.element.rethinkdb._bluebird.all)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>any (promises)](#apidoc.element.rethinkdb._bluebird.any)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>attempt (fn, args, ctx)](#apidoc.element.rethinkdb._bluebird.attempt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>bind (thisArg, value)](#apidoc.element.rethinkdb._bluebird.bind)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>cast (obj)](#apidoc.element.rethinkdb._bluebird.cast)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>defer ()](#apidoc.element.rethinkdb._bluebird.defer)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>delay (value, ms)](#apidoc.element.rethinkdb._bluebird.delay)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>each (promises, fn)](#apidoc.element.rethinkdb._bluebird.each)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>filter (promises, fn, options)](#apidoc.element.rethinkdb._bluebird.filter)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>fromNode (fn)](#apidoc.element.rethinkdb._bluebird.fromNode)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>fulfilled (obj)](#apidoc.element.rethinkdb._bluebird.fulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>getNewLibraryCopy ()](#apidoc.element.rethinkdb._bluebird.getNewLibraryCopy)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>hasLongStackTraces ()](#apidoc.element.rethinkdb._bluebird.hasLongStackTraces)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>is (val)](#apidoc.element.rethinkdb._bluebird.is)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>join ()](#apidoc.element.rethinkdb._bluebird.join)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>longStackTraces ()](#apidoc.element.rethinkdb._bluebird.longStackTraces)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>map (promises, fn, options, _filter)](#apidoc.element.rethinkdb._bluebird.map)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>method (fn)](#apidoc.element.rethinkdb._bluebird.method)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>noConflict ()](#apidoc.element.rethinkdb._bluebird.noConflict)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.rethinkdb._bluebird.onPossiblyUnhandledRejection)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.rethinkdb._bluebird.onUnhandledRejectionHandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>pending ()](#apidoc.element.rethinkdb._bluebird.pending)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>promisify (fn, receiver)](#apidoc.element.rethinkdb._bluebird.promisify)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>promisifyAll (target, options)](#apidoc.element.rethinkdb._bluebird.promisifyAll)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>props (promises)](#apidoc.element.rethinkdb._bluebird.props)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>race (promises)](#apidoc.element.rethinkdb._bluebird.race)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.rethinkdb._bluebird.reduce)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>reject (reason)](#apidoc.element.rethinkdb._bluebird.reject)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>rejected (reason)](#apidoc.element.rethinkdb._bluebird.rejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>resolve (obj)](#apidoc.element.rethinkdb._bluebird.resolve)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>setScheduler (fn)](#apidoc.element.rethinkdb._bluebird.setScheduler)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>settle (promises)](#apidoc.element.rethinkdb._bluebird.settle)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>some (promises, howMany)](#apidoc.element.rethinkdb._bluebird.some)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>spawn (generatorFunction)](#apidoc.element.rethinkdb._bluebird.spawn)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>try (fn, args, ctx)](#apidoc.element.rethinkdb._bluebird.try)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>using ()](#apidoc.element.rethinkdb._bluebird.using)
1.  string <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>version

#### [module rethinkdb._bluebird.AggregateError](#apidoc.module.rethinkdb._bluebird.AggregateError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError.AggregateError)

#### [module rethinkdb._bluebird.AggregateError.prototype](#apidoc.module.rethinkdb._bluebird.AggregateError.prototype)
1.  boolean <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>isOperational
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>every ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.every)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>filter ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.filter)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>forEach ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>indexOf ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>join ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.join)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>map ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.map)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>pop ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.pop)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>push ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.push)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reduce ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reverse ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>shift ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.shift)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>slice ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.slice)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>some ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.some)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>sort ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.sort)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>toString ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.toString)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>unshift ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.unshift)
1.  number <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>length

#### [module rethinkdb._bluebird.CancellationError](#apidoc.module.rethinkdb._bluebird.CancellationError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError.CancellationError)

#### [module rethinkdb._bluebird.CancellationError.prototype](#apidoc.module.rethinkdb._bluebird.CancellationError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.CancellationError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.CancellationError.prototype.constructor)

#### [module rethinkdb._bluebird.OperationalError](#apidoc.module.rethinkdb._bluebird.OperationalError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError.OperationalError)

#### [module rethinkdb._bluebird.OperationalError.prototype](#apidoc.module.rethinkdb._bluebird.OperationalError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.OperationalError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.OperationalError.prototype.constructor)

#### [module rethinkdb._bluebird.PromiseInspection](#apidoc.module.rethinkdb._bluebird.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection.PromiseInspection)

#### [module rethinkdb._bluebird.PromiseInspection.prototype](#apidoc.module.rethinkdb._bluebird.PromiseInspection.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>error ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.error)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isResolved)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>reason ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.reason)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>value ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.value)

#### [module rethinkdb._bluebird.TimeoutError](#apidoc.module.rethinkdb._bluebird.TimeoutError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError.TimeoutError)

#### [module rethinkdb._bluebird.TimeoutError.prototype](#apidoc.module.rethinkdb._bluebird.TimeoutError.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError.prototype.constructor)

#### [module rethinkdb._bluebird._SomePromiseArray](#apidoc.module.rethinkdb._bluebird._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>_SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray._SomePromiseArray)

#### [module rethinkdb._bluebird._SomePromiseArray.prototype](#apidoc.module.rethinkdb._bluebird._SomePromiseArray.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._canPossiblyFulfill)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._fulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._getRangeError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._init)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._rejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._resolveEmptyArray)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.howMany)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>init ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.init)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setHowMany)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setUnwrap)

#### [module rethinkdb._bluebird.coroutine](#apidoc.module.rethinkdb._bluebird.coroutine)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine.coroutine)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.coroutine.</span>addYieldHandler (fn)](#apidoc.element.rethinkdb._bluebird.coroutine.addYieldHandler)

#### [module rethinkdb._bluebird.prototype](#apidoc.module.rethinkdb._bluebird.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_addCallbacks ( fulfill, reject, progress, promise, receiver, domain )](#apidoc.element.rethinkdb._bluebird.prototype._addCallbacks)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_attachExtraTrace (error, ignoreSelf)](#apidoc.element.rethinkdb._bluebird.prototype._attachExtraTrace)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_boundValue ()](#apidoc.element.rethinkdb._bluebird.prototype._boundValue)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cancel (reason)](#apidoc.element.rethinkdb._bluebird.prototype._cancel)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._cancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_captureStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._captureStackTrace)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cleanValues ()](#apidoc.element.rethinkdb._bluebird.prototype._cleanValues)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_clearCallbackDataAtIndex (index)](#apidoc.element.rethinkdb._bluebird.prototype._clearCallbackDataAtIndex)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_doProgressWith (progression)](#apidoc.element.rethinkdb._bluebird.prototype._doProgressWith)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_ensurePossibleRejectionHandled ()](#apidoc.element.rethinkdb._bluebird.prototype._ensurePossibleRejectionHandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_followee ()](#apidoc.element.rethinkdb._bluebird.prototype._followee)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfill (value)](#apidoc.element.rethinkdb._bluebird.prototype._fulfill)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfillUnchecked (value)](#apidoc.element.rethinkdb._bluebird.prototype._fulfillUnchecked)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfillmentHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._fulfillmentHandlerAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_getCarriedStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._getCarriedStackTrace)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_getDisposer ()](#apidoc.element.rethinkdb._bluebird.prototype._getDisposer)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_ignoreRejections ()](#apidoc.element.rethinkdb._bluebird.prototype._ignoreRejections)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isBound ()](#apidoc.element.rethinkdb._bluebird.prototype._isBound)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isCarryingStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._isCarryingStackTrace)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isDisposable ()](#apidoc.element.rethinkdb._bluebird.prototype._isDisposable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFinal ()](#apidoc.element.rethinkdb._bluebird.prototype._isFinal)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFollowing ()](#apidoc.element.rethinkdb._bluebird.prototype._isFollowing)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFollowingOrFulfilledOrRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._isFollowingOrFulfilledOrRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype._isFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._isMigrated)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isPending ()](#apidoc.element.rethinkdb._bluebird.prototype._isPending)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._isRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isRejectionUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._isRejectionUnhandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isResolved ()](#apidoc.element.rethinkdb._bluebird.prototype._isResolved)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._isSettlePromisesQueued)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isUnhandledRejectionNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._isUnhandledRejectionNotified)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_length ()](#apidoc.element.rethinkdb._bluebird.prototype._length)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_migrateCallbacks (follower, index)](#apidoc.element.rethinkdb._bluebird.prototype._migrateCallbacks)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_notifyUnhandledRejection ()](#apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejection)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_notifyUnhandledRejectionIsHandled ()](#apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejectionIsHandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_passThroughHandler (handler, isFinally)](#apidoc.element.rethinkdb._bluebird.prototype._passThroughHandler)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_peekContext ()](#apidoc.element.rethinkdb._bluebird.prototype._peekContext)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_popContext ()](#apidoc.element.rethinkdb._bluebird.prototype._popContext)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progress (progressValue)](#apidoc.element.rethinkdb._bluebird.prototype._progress)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progressHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._progressHandlerAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progressUnchecked (progressValue)](#apidoc.element.rethinkdb._bluebird.prototype._progressUnchecked)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_promiseAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._promiseAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_propagateFrom (parent, flags)](#apidoc.element.rethinkdb._bluebird.prototype._propagateFrom)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_proxyPromiseArray (promiseArray, index)](#apidoc.element.rethinkdb._bluebird.prototype._proxyPromiseArray)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_pushContext ()](#apidoc.element.rethinkdb._bluebird.prototype._pushContext)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_queueSettlePromises ()](#apidoc.element.rethinkdb._bluebird.prototype._queueSettlePromises)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_reason ()](#apidoc.element.rethinkdb._bluebird.prototype._reason)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_receiverAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._receiverAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_reject (reason, carriedStackTrace)](#apidoc.element.rethinkdb._bluebird.prototype._reject)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectCallback (reason, synchronous, shouldNotMarkOriginatingFromRejection)](#apidoc.element.rethinkdb._bluebird.prototype._rejectCallback)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectUnchecked (reason, trace)](#apidoc.element.rethinkdb._bluebird.prototype._rejectUnchecked)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectUncheckedCheckError (reason)](#apidoc.element.rethinkdb._bluebird.prototype._rejectUncheckedCheckError)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectionHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._rejectionHandlerAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveCallback (value, shouldBind)](#apidoc.element.rethinkdb._bluebird.prototype._resolveCallback)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveFromResolver (resolver)](#apidoc.element.rethinkdb._bluebird.prototype._resolveFromResolver)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveFromSyncValue (value)](#apidoc.element.rethinkdb._bluebird.prototype._resolveFromSyncValue)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setBoundTo (obj)](#apidoc.element.rethinkdb._bluebird.prototype._setBoundTo)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._setCancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setCarriedStackTrace (capturedTrace)](#apidoc.element.rethinkdb._bluebird.prototype._setCarriedStackTrace)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setDisposable (disposer)](#apidoc.element.rethinkdb._bluebird.prototype._setDisposable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFollowee (promise)](#apidoc.element.rethinkdb._bluebird.prototype._setFollowee)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFollowing ()](#apidoc.element.rethinkdb._bluebird.prototype._setFollowing)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype._setFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setIsFinal ()](#apidoc.element.rethinkdb._bluebird.prototype._setIsFinal)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setIsMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._setIsMigrated)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setLength (len)](#apidoc.element.rethinkdb._bluebird.prototype._setLength)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setProxyHandlers (receiver, promiseSlotValue)](#apidoc.element.rethinkdb._bluebird.prototype._setProxyHandlers)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._setRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setRejectionIsUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._setRejectionIsUnhandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._setSettlePromisesQueued)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setUnhandledRejectionIsNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._setUnhandledRejectionIsNotified)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAt)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseAtPostResolution (index)](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAtPostResolution)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseFromHandler ( handler, receiver, value, promise )](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseFromHandler)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromises ()](#apidoc.element.rethinkdb._bluebird.prototype._settlePromises)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_target ()](#apidoc.element.rethinkdb._bluebird.prototype._target)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_then ( didFulfill, didReject, didProgress, receiver, internalData )](#apidoc.element.rethinkdb._bluebird.prototype._then)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetCancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetDisposable ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetDisposable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetIsMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetIsMigrated)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetRejectionIsUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetRejectionIsUnhandled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetSettlePromisesQueued)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetUnhandledRejectionIsNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetUnhandledRejectionIsNotified)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_value ()](#apidoc.element.rethinkdb._bluebird.prototype._value)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_warn (message)](#apidoc.element.rethinkdb._bluebird.prototype._warn)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>all ()](#apidoc.element.rethinkdb._bluebird.prototype.all)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>any ()](#apidoc.element.rethinkdb._bluebird.prototype.any)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>asCallback (nodeback, options)](#apidoc.element.rethinkdb._bluebird.prototype.asCallback)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>bind (thisArg)](#apidoc.element.rethinkdb._bluebird.prototype.bind)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>call (methodName)](#apidoc.element.rethinkdb._bluebird.prototype.call)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>cancel (reason)](#apidoc.element.rethinkdb._bluebird.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>cancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.cancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>catch (fn)](#apidoc.element.rethinkdb._bluebird.prototype.catch)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>caught (fn)](#apidoc.element.rethinkdb._bluebird.prototype.caught)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>delay (ms)](#apidoc.element.rethinkdb._bluebird.prototype.delay)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>disposer (fn)](#apidoc.element.rethinkdb._bluebird.prototype.disposer)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>done (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.done)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>each (fn)](#apidoc.element.rethinkdb._bluebird.prototype.each)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>error (fn)](#apidoc.element.rethinkdb._bluebird.prototype.error)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>filter (fn, options)](#apidoc.element.rethinkdb._bluebird.prototype.filter)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>finally (handler)](#apidoc.element.rethinkdb._bluebird.prototype.finally)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>fork (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.fork)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>get (propertyName)](#apidoc.element.rethinkdb._bluebird.prototype.get)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.isCancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isPending ()](#apidoc.element.rethinkdb._bluebird.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isRejected ()](#apidoc.element.rethinkdb._bluebird.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isResolved ()](#apidoc.element.rethinkdb._bluebird.prototype.isResolved)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>lastly (handler)](#apidoc.element.rethinkdb._bluebird.prototype.lastly)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>map (fn, options)](#apidoc.element.rethinkdb._bluebird.prototype.map)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>nodeify (nodeback, options)](#apidoc.element.rethinkdb._bluebird.prototype.nodeify)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>progressed (handler)](#apidoc.element.rethinkdb._bluebird.prototype.progressed)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>props ()](#apidoc.element.rethinkdb._bluebird.prototype.props)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>race ()](#apidoc.element.rethinkdb._bluebird.prototype.race)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reason ()](#apidoc.element.rethinkdb._bluebird.prototype.reason)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reduce (fn, initialValue)](#apidoc.element.rethinkdb._bluebird.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reflect ()](#apidoc.element.rethinkdb._bluebird.prototype.reflect)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>return (value)](#apidoc.element.rethinkdb._bluebird.prototype.return)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>settle ()](#apidoc.element.rethinkdb._bluebird.prototype.settle)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>some (howMany)](#apidoc.element.rethinkdb._bluebird.prototype.some)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>spread (didFulfill, didReject)](#apidoc.element.rethinkdb._bluebird.prototype.spread)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>tap (handler)](#apidoc.element.rethinkdb._bluebird.prototype.tap)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>then (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.then)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>thenReturn (value)](#apidoc.element.rethinkdb._bluebird.prototype.thenReturn)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>thenThrow (reason)](#apidoc.element.rethinkdb._bluebird.prototype.thenThrow)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>throw (reason)](#apidoc.element.rethinkdb._bluebird.prototype.throw)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>timeout (ms, message)](#apidoc.element.rethinkdb._bluebird.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>toJSON ()](#apidoc.element.rethinkdb._bluebird.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>toString ()](#apidoc.element.rethinkdb._bluebird.prototype.toString)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>uncancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.uncancellable)
1.  [function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>value ()](#apidoc.element.rethinkdb._bluebird.prototype.value)

#### [module rethinkdb.cursor](#apidoc.module.rethinkdb.cursor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>AtomFeed ()](#apidoc.element.rethinkdb.cursor.AtomFeed)
1.  [function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>Cursor ()](#apidoc.element.rethinkdb.cursor.Cursor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>Feed ()](#apidoc.element.rethinkdb.cursor.Feed)
1.  [function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>OrderByLimitFeed ()](#apidoc.element.rethinkdb.cursor.OrderByLimitFeed)
1.  [function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>makeIterable (response)](#apidoc.element.rethinkdb.cursor.makeIterable)

#### [module rethinkdb.net](#apidoc.module.rethinkdb.net)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>connect ()](#apidoc.element.rethinkdb.net.connect)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>isConnection (connection)](#apidoc.element.rethinkdb.net.isConnection)

#### [module rethinkdb.net.Connection](#apidoc.module.rethinkdb.net.Connection)
1.  boolean <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.Connection.EventEmitter)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>init ()](#apidoc.element.rethinkdb.net.Connection.init)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.Connection.listenerCount)
1.  number <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>__super__

#### [module rethinkdb.net.Connection.prototype](#apidoc.module.rethinkdb.net.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_continueQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._continueQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_data (buf)](#apidoc.element.rethinkdb.net.Connection.prototype._data)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_delQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._delQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_endQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._endQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_processResponse (response, token)](#apidoc.element.rethinkdb.net.Connection.prototype._processResponse)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_sendQuery (query)](#apidoc.element.rethinkdb.net.Connection.prototype._sendQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_start (term, cb, opts)](#apidoc.element.rethinkdb.net.Connection.prototype._start)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.Connection.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.Connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.Connection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>isOpen ()](#apidoc.element.rethinkdb.net.Connection.prototype.isOpen)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>noreplyWait ()](#apidoc.element.rethinkdb.net.Connection.prototype.noreplyWait)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>reconnect ()](#apidoc.element.rethinkdb.net.Connection.prototype.reconnect)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>server ()](#apidoc.element.rethinkdb.net.Connection.prototype.server)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>use ()](#apidoc.element.rethinkdb.net.Connection.prototype.use)
1.  number <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>DEFAULT_PORT
1.  number <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>DEFAULT_TIMEOUT
1.  string <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>DEFAULT_AUTH_KEY
1.  string <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>DEFAULT_HOST

#### [module rethinkdb.net.HttpConnection](#apidoc.module.rethinkdb.net.HttpConnection)
1.  boolean <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection.HttpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.HttpConnection.EventEmitter)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>init ()](#apidoc.element.rethinkdb.net.HttpConnection.init)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>isAvailable ()](#apidoc.element.rethinkdb.net.HttpConnection.isAvailable)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.HttpConnection.listenerCount)
1.  number <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>__super__

#### [module rethinkdb.net.HttpConnection.prototype](#apidoc.module.rethinkdb.net.HttpConnection.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>_writeQuery (token, data)](#apidoc.element.rethinkdb.net.HttpConnection.prototype._writeQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.HttpConnection.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.HttpConnection.prototype.close)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>write (chunk, token)](#apidoc.element.rethinkdb.net.HttpConnection.prototype.write)
1.  string <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>DEFAULT_PROTOCOL

#### [module rethinkdb.net.TcpConnection](#apidoc.module.rethinkdb.net.TcpConnection)
1.  boolean <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.</span>TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection.TcpConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.TcpConnection.EventEmitter)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>init ()](#apidoc.element.rethinkdb.net.TcpConnection.init)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>isAvailable ()](#apidoc.element.rethinkdb.net.TcpConnection.isAvailable)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.TcpConnection.listenerCount)
1.  number <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>__super__

#### [module rethinkdb.net.TcpConnection.prototype](#apidoc.module.rethinkdb.net.TcpConnection.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>_writeQuery (token, data)](#apidoc.element.rethinkdb.net.TcpConnection.prototype._writeQuery)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>clientAddress ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.clientAddress)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>clientPort ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.clientPort)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.close)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>write (chunk)](#apidoc.element.rethinkdb.net.TcpConnection.prototype.write)

#### [module rethinkdb.util](#apidoc.module.rethinkdb.util)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>ar (fun)](#apidoc.element.rethinkdb.util.ar)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>aropt (fun)](#apidoc.element.rethinkdb.util.aropt)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>errorClass (errorType)](#apidoc.element.rethinkdb.util.errorClass)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>fromCamelCase (token)](#apidoc.element.rethinkdb.util.fromCamelCase)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkAtom (response, opts)](#apidoc.element.rethinkdb.util.mkAtom)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkErr (ErrClass, response, root)](#apidoc.element.rethinkdb.util.mkErr)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkSeq (response, opts)](#apidoc.element.rethinkdb.util.mkSeq)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>recursivelyConvertPseudotype (obj, opts)](#apidoc.element.rethinkdb.util.recursivelyConvertPseudotype)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>toArrayBuffer (node_buffer)](#apidoc.element.rethinkdb.util.toArrayBuffer)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>toCamelCase (token)](#apidoc.element.rethinkdb.util.toCamelCase)
1.  [function <span class="apidocSignatureSpan">rethinkdb.util.</span>varar (min, max, fun)](#apidoc.element.rethinkdb.util.varar)



# <a name="apidoc.module.rethinkdb"></a>[module rethinkdb](#apidoc.module.rethinkdb)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAuthError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError)
- description and source-code
```javascript
function ReqlAuthError() {
  return ReqlAuthError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlAvailabilityError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError)
- description and source-code
```javascript
function ReqlAvailabilityError() {
  return ReqlAvailabilityError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError)
- description and source-code
```javascript
function ReqlCompileError() {
  return ReqlCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError)
- description and source-code
```javascript
function ReqlDriverCompileError() {
  return ReqlDriverCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError)
- description and source-code
```javascript
function ReqlError(msg, term, frames) {
  this.name = this.constructor.name;
  this.msg = msg;
  this.frames = frames != null ? frames.slice(0) : void 0;
  if (term != null) {
    if (msg[msg.length - 1] === '.') {
      this.message = (msg.slice(0, msg.length - 1)) + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter
.prototype.printCarrots(term, frames));
    } else {
      this.message = msg + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter.prototype.printCarrots
(term, frames));
    }
  } else {
    this.message = "" + msg;
  }
  if (Error.captureStackTrace != null) {
    Error.captureStackTrace(this, this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlInternalError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError)
- description and source-code
```javascript
function ReqlInternalError() {
  return ReqlInternalError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlNonExistenceError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError)
- description and source-code
```javascript
function ReqlNonExistenceError() {
  return ReqlNonExistenceError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpFailedError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError)
- description and source-code
```javascript
function ReqlOpFailedError() {
  return ReqlOpFailedError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError)
- description and source-code
```javascript
function ReqlOpIndeterminateError() {
  return ReqlOpIndeterminateError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlPermissionError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError)
- description and source-code
```javascript
function ReqlPermissionError() {
  return ReqlPermissionError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlQueryLogicError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError)
- description and source-code
```javascript
function ReqlQueryLogicError() {
  return ReqlQueryLogicError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlResourceLimitError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError)
- description and source-code
```javascript
function ReqlResourceLimitError() {
  return ReqlResourceLimitError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlRuntimeError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlServerCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError)
- description and source-code
```javascript
function ReqlServerCompileError() {
  return ReqlServerCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlTimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError)
- description and source-code
```javascript
function ReqlTimeoutError() {
  return ReqlTimeoutError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlUserError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError)
- description and source-code
```javascript
function ReqlUserError() {
  return ReqlUserError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlClientError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>Error.RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.ISO8601"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>ISO8601 ()](#apidoc.element.rethinkdb.ISO8601)
- description and source-code
```javascript
ISO8601 = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird (resolver)](#apidoc.element.rethinkdb._bluebird)
- description and source-code
```javascript
function Promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("the promise constructor requires a resolver function\u000a\u000a    See http://goo.gl/EC22Yn\u000a");
    }
    if (this.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/KsIlge\u000a");
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._progressHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._settledValue = undefined;
    if (resolver !== INTERNAL) this._resolveFromResolver(resolver);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.CancellationError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.OperationalError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValue = promise._settledValue;
    }
    else {
        this._bitField = 0;
        this._settledValue = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.TimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird._SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.coroutine"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird.coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine)
- description and source-code
```javascript
_bluebird.coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/6Vqhm0\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        spawn._generator = generator;
        spawn._next(undefined);
        return spawn.promise();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.add"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>add ()](#apidoc.element.rethinkdb.add)
- description and source-code
```javascript
add = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Add, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.and"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>and ()](#apidoc.element.rethinkdb.and)
- description and source-code
```javascript
and = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(And, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.april"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>april {{signature}}](#apidoc.element.rethinkdb.april)
- description and source-code
```javascript
r.april
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.args"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>args ()](#apidoc.element.rethinkdb.args)
- description and source-code
```javascript
args = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Args, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.asc"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>asc ()](#apidoc.element.rethinkdb.asc)
- description and source-code
```javascript
asc = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Asc, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.august"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>august {{signature}}](#apidoc.element.rethinkdb.august)
- description and source-code
```javascript
r.august
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.avg"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>avg ()](#apidoc.element.rethinkdb.avg)
- description and source-code
```javascript
avg = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Avg, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.binary"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>binary ()](#apidoc.element.rethinkdb.binary)
- description and source-code
```javascript
binary = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (args.length !== fun.length) {
    throw new err.ReqlDriverCompileError("Expected " + fun.length + " argument" + (plural(fun.length)) + " but found " + args.length
 + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.branch"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>branch ()](#apidoc.element.rethinkdb.branch)
- description and source-code
```javascript
branch = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Branch, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.ceil"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>ceil ()](#apidoc.element.rethinkdb.ceil)
- description and source-code
```javascript
ceil = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Ceil, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.circle"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>circle ()](#apidoc.element.rethinkdb.circle)
- description and source-code
```javascript
circle = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.connect"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>connect ()](#apidoc.element.rethinkdb.connect)
- description and source-code
```javascript
connect = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.contains"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>contains ()](#apidoc.element.rethinkdb.contains)
- description and source-code
```javascript
contains = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Contains, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.count"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>count ()](#apidoc.element.rethinkdb.count)
- description and source-code
```javascript
count = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Count, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.db"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>db ()](#apidoc.element.rethinkdb.db)
- description and source-code
```javascript
db = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Db, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.dbCreate"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>dbCreate ()](#apidoc.element.rethinkdb.dbCreate)
- description and source-code
```javascript
dbCreate = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(DbCreate, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.dbDrop"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>dbDrop ()](#apidoc.element.rethinkdb.dbDrop)
- description and source-code
```javascript
dbDrop = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(DbDrop, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.dbList"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>dbList ()](#apidoc.element.rethinkdb.dbList)
- description and source-code
```javascript
dbList = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(DbList, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.december"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>december {{signature}}](#apidoc.element.rethinkdb.december)
- description and source-code
```javascript
r.december
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.desc"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>desc ()](#apidoc.element.rethinkdb.desc)
- description and source-code
```javascript
desc = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Desc, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.distance"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>distance ()](#apidoc.element.rethinkdb.distance)
- description and source-code
```javascript
distance = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.distinct"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>distinct ()](#apidoc.element.rethinkdb.distinct)
- description and source-code
```javascript
distinct = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Distinct, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.div"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>div ()](#apidoc.element.rethinkdb.div)
- description and source-code
```javascript
div = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Div, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.do"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>do ()](#apidoc.element.rethinkdb.do)
- description and source-code
```javascript
do = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.epochTime"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>epochTime ()](#apidoc.element.rethinkdb.epochTime)
- description and source-code
```javascript
epochTime = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(EpochTime, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.eq"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>eq ()](#apidoc.element.rethinkdb.eq)
- description and source-code
```javascript
eq = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Eq, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.error"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>error ()](#apidoc.element.rethinkdb.error)
- description and source-code
```javascript
error = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(UserError, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.expr"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>expr ()](#apidoc.element.rethinkdb.expr)
- description and source-code
```javascript
expr = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.february"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>february {{signature}}](#apidoc.element.rethinkdb.february)
- description and source-code
```javascript
r.february
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.floor"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>floor ()](#apidoc.element.rethinkdb.floor)
- description and source-code
```javascript
floor = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Floor, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.friday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>friday {{signature}}](#apidoc.element.rethinkdb.friday)
- description and source-code
```javascript
r.friday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.ge"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>ge ()](#apidoc.element.rethinkdb.ge)
- description and source-code
```javascript
ge = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Ge, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.geojson"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>geojson ()](#apidoc.element.rethinkdb.geojson)
- description and source-code
```javascript
geojson = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Geojson, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.grant"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>grant ()](#apidoc.element.rethinkdb.grant)
- description and source-code
```javascript
grant = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Grant, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.group"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>group ()](#apidoc.element.rethinkdb.group)
- description and source-code
```javascript
group = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Group, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.gt"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>gt ()](#apidoc.element.rethinkdb.gt)
- description and source-code
```javascript
gt = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Gt, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.http"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>http ()](#apidoc.element.rethinkdb.http)
- description and source-code
```javascript
http = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.info"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>info ()](#apidoc.element.rethinkdb.info)
- description and source-code
```javascript
info = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Info, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.intersects"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>intersects ()](#apidoc.element.rethinkdb.intersects)
- description and source-code
```javascript
intersects = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Intersects, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.january"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>january {{signature}}](#apidoc.element.rethinkdb.january)
- description and source-code
```javascript
r.january
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.js"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>js ()](#apidoc.element.rethinkdb.js)
- description and source-code
```javascript
js = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.json"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>json ()](#apidoc.element.rethinkdb.json)
- description and source-code
```javascript
json = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Json, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.july"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>july {{signature}}](#apidoc.element.rethinkdb.july)
- description and source-code
```javascript
r.july
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.june"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>june {{signature}}](#apidoc.element.rethinkdb.june)
- description and source-code
```javascript
r.june
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.le"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>le ()](#apidoc.element.rethinkdb.le)
- description and source-code
```javascript
le = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Le, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.line"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>line ()](#apidoc.element.rethinkdb.line)
- description and source-code
```javascript
line = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Line, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.literal"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>literal ()](#apidoc.element.rethinkdb.literal)
- description and source-code
```javascript
literal = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Literal, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.lt"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>lt ()](#apidoc.element.rethinkdb.lt)
- description and source-code
```javascript
lt = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Lt, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.map"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>map ()](#apidoc.element.rethinkdb.map)
- description and source-code
```javascript
map = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.march"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>march {{signature}}](#apidoc.element.rethinkdb.march)
- description and source-code
```javascript
r.march
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.max"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>max ()](#apidoc.element.rethinkdb.max)
- description and source-code
```javascript
max = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Max, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.maxval"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>maxval {{signature}}](#apidoc.element.rethinkdb.maxval)
- description and source-code
```javascript
r.maxval
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.may"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>may {{signature}}](#apidoc.element.rethinkdb.may)
- description and source-code
```javascript
r.may
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.min"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>min ()](#apidoc.element.rethinkdb.min)
- description and source-code
```javascript
min = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Min, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.minval"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>minval {{signature}}](#apidoc.element.rethinkdb.minval)
- description and source-code
```javascript
r.minval
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.mod"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>mod ()](#apidoc.element.rethinkdb.mod)
- description and source-code
```javascript
mod = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Mod, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.monday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>monday {{signature}}](#apidoc.element.rethinkdb.monday)
- description and source-code
```javascript
r.monday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.mul"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>mul ()](#apidoc.element.rethinkdb.mul)
- description and source-code
```javascript
mul = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Mul, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.ne"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>ne ()](#apidoc.element.rethinkdb.ne)
- description and source-code
```javascript
ne = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Ne, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>net.Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection)
- description and source-code
```javascript
function Connection(host, callback) {
  var conCallback, errCallback;
  if (typeof host === 'undefined') {
    host = {};
  } else if (typeof host === 'string') {
    host = {
      host: host
    };
  }
  this.host = host.host || this.DEFAULT_HOST;
  this.port = host.port || this.DEFAULT_PORT;
  this.db = host.db;
  this.authKey = host.authKey || this.DEFAULT_AUTH_KEY;
  this.timeout = host.timeout || this.DEFAULT_TIMEOUT;
  if (typeof host.ssl === 'boolean' && host.ssl) {
    this.ssl = {};
  } else if (typeof host.ssl === 'object') {
    this.ssl = host.ssl;
  } else {
    this.ssl = false;
  }
  this.outstandingCallbacks = {};
  this.nextToken = 1;
  this.open = false;
  this.closing = false;
  this.buffer = new Buffer(0);
  this._events = this._events || {};
  errCallback = (function(_this) {
    return function(e) {
      _this.removeListener('connect', conCallback);
      if (e instanceof err.ReqlError) {
        return callback(e);
      } else {
        return callback(new err.ReqlDriverError("Could not connect to " + _this.host + ":" + _this.port + ".\n" + e.message));
      }
    };
  })(this);
  this.once('error', errCallback);
  conCallback = (function(_this) {
    return function() {
      _this.removeListener('error', errCallback);
      _this.open = true;
      return callback(null, _this);
    };
  })(this);
  this.once('connect', conCallback);
  this._closePromise = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>net.HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection)
- description and source-code
```javascript
function HttpConnection(host, callback) {
  var protocol, url, xhr;
  if (!HttpConnection.isAvailable()) {
    throw new err.ReqlDriverError("XMLHttpRequest is not available in this environment");
  }
  HttpConnection.__super__.constructor.call(this, host, callback);
  protocol = host.protocol === 'https' ? 'https' : this.DEFAULT_PROTOCOL;
  url = protocol + "://" + this.host + ":" + this.port + host.pathname + "ajax/reql/";
  xhr = new XMLHttpRequest;
  xhr.open("POST", url + ("open-new-connection?cacheBuster=" + (Math.random())), true);
  xhr.responseType = "text";
  xhr.onreadystatechange = (function(_this) {
    return function(e) {
      if (xhr.readyState === 4) {
        if (xhr.status === 200) {
          _this._url = url;
          _this._connId = xhr.response;
          return _this.emit('connect');
        } else {
          return _this.emit('error', new err.ReqlDriverError("XHR error, http status " + xhr.status + "."));
        }
      }
    };
  })(this);
  xhr.send();
  this.xhr = xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>net.TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection)
- description and source-code
```javascript
function TcpConnection(host, callback) {
  var timeout;
  if (!TcpConnection.isAvailable()) {
    throw new err.ReqlDriverError("TCP sockets are not available in this environment");
  }
  TcpConnection.__super__.constructor.call(this, host, callback);
  if (this.ssl) {
    this.ssl.host = this.host;
    this.ssl.port = this.port;
    this.rawSocket = tls.connect(this.ssl);
  } else {
    this.rawSocket = net.connect(this.port, this.host);
  }
  this.rawSocket.setNoDelay();
  this.rawSocket.setKeepAlive(true);
  timeout = setTimeout(((function(_this) {
    return function() {
      _this.rawSocket.destroy();
      return _this.emit('error', new err.ReqlTimeoutError("Could not connect to " + _this.host + ":" + _this.port + ", operation
 timed out."));
    };
  })(this)), this.timeout * 1000);
  this.rawSocket.once('error', (function(_this) {
    return function() {
      return clearTimeout(timeout);
    };
  })(this));
  this.rawSocket.once('connect', (function(_this) {
    return function() {
      var auth_i, auth_r, auth_salt, client_first_message_bare, compare_digest, handshake_callback, handshake_error, max, message
, min, nullbyte, pbkdf2_hmac, protocol, r_string, server_first_message, server_signature, state, version, xor_bytes;
      version = new Buffer(4);
      version.writeUInt32LE(protoVersion, 0);
      protocol = new Buffer(4);
      protocol.writeUInt32LE(protoProtocol, 0);
      r_string = new Buffer(crypto.randomBytes(18)).toString('base64');
      _this.rawSocket.user = host["user"];
      _this.rawSocket.password = host["password"];
      if (_this.rawSocket.user === void 0) {
        _this.rawSocket.user = "admin";
      }
      if (_this.rawSocket.password === void 0) {
        _this.rawSocket.password = "";
      }
      client_first_message_bare = "n=" + _this.rawSocket.user + ",r=" + r_string;
      message = JSON.stringify({
        protocol_version: protoVersionNumber,
        authentication_method: "SCRAM-SHA-256",
        authentication: "n,," + client_first_message_bare
      });
      nullbyte = new Buffer('\0', "binary");
      _this.rawSocket.write(Buffer.concat([version, Buffer(message.toString()), nullbyte]));
      state = 1;
      min = 0;
      max = 0;
      server_first_message = "";
      server_signature = "";
      auth_r = "";
      auth_salt = "";
      auth_i = 0;
      xor_bytes = function(a, b) {
        var i, k, len, ref, res;
        res = [];
        len = Math.min(a.length, b.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          res.push(a[i] ^ b[i]);
        }
        return new Buffer(res);
      };
      pbkdf2_hmac = function(password, salt, iterations) {
        var c, cache_string, k, mac, ref, t, u;
        cache_string = password.toString("base64") + "," + salt.toString("base64") + "," + iterations.toString();
        if (pbkdf2_cache[cache_string]) {
          return pbkdf2_cache[cache_string];
        }
        mac = crypto.createHmac("sha256", password);
        mac.update(salt);
        mac.update("\x00\x00\x00\x01");
        u = mac.digest();
        t = u;
        for (c = k = 0, ref = iterations - 1; 0 <= ref ? k < ref : k > ref; c = 0 <= ref ? ++k : --k) {
          mac = crypto.createHmac("sha256", password);
          mac.update(t);
          t = mac.digest();
          u = xor_bytes(u, t);
        }
        pbkdf2_cache[cache_string] = u;
        return u;
      };
      compare_digest = function(a, b) {
        var i, k, left, len, ref, result, right;
        left = void 0;
        right = b;
        result = void 0;
        if (a.length === b.length) {
          left = a;
          result = 0;
        }
        if (a.length !== b.length) {
          left = b;
          result = 1;
        }
        len = Math.min(left.length, right.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          result |= left[i] ^ right[i];
        }
        return result === 0;
      };
      handshake_error = function(code, message) {
        if ((10 <= code & ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.not"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>not ()](#apidoc.element.rethinkdb.not)
- description and source-code
```javascript
not = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Not, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.november"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>november {{signature}}](#apidoc.element.rethinkdb.november)
- description and source-code
```javascript
r.november
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.now"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>now ()](#apidoc.element.rethinkdb.now)
- description and source-code
```javascript
now = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Now, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.object"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>object ()](#apidoc.element.rethinkdb.object)
- description and source-code
```javascript
object = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Object_, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.october"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>october {{signature}}](#apidoc.element.rethinkdb.october)
- description and source-code
```javascript
r.october
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.or"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>or ()](#apidoc.element.rethinkdb.or)
- description and source-code
```javascript
or = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Or, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.point"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>point ()](#apidoc.element.rethinkdb.point)
- description and source-code
```javascript
point = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Point, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.polygon"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>polygon ()](#apidoc.element.rethinkdb.polygon)
- description and source-code
```javascript
polygon = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Polygon, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.random"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>random ()](#apidoc.element.rethinkdb.random)
- description and source-code
```javascript
random = function () {
  var limits, limitsAndOpts, opts, perhapsOptDict;
  limitsAndOpts = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  opts = {};
  limits = limitsAndOpts;
  perhapsOptDict = limitsAndOpts[limitsAndOpts.length - 1];
  if (perhapsOptDict && ((Object.prototype.toString.call(perhapsOptDict) === '[object Object]') && !(perhapsOptDict instanceof TermBase
))) {
    opts = perhapsOptDict;
    limits = limitsAndOpts.slice(0, limitsAndOpts.length - 1);
  }
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Random, [opts].concat(slice.call(limits)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.range"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>range ()](#apidoc.element.rethinkdb.range)
- description and source-code
```javascript
range = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Range, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.reduce"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>reduce ()](#apidoc.element.rethinkdb.reduce)
- description and source-code
```javascript
reduce = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Reduce, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.round"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>round ()](#apidoc.element.rethinkdb.round)
- description and source-code
```javascript
round = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Round, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.row"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>row {{signature}}](#apidoc.element.rethinkdb.row)
- description and source-code
```javascript
r.row
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.saturday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>saturday {{signature}}](#apidoc.element.rethinkdb.saturday)
- description and source-code
```javascript
r.saturday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.september"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>september {{signature}}](#apidoc.element.rethinkdb.september)
- description and source-code
```javascript
r.september
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.sub"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>sub ()](#apidoc.element.rethinkdb.sub)
- description and source-code
```javascript
sub = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Sub, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.sum"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>sum ()](#apidoc.element.rethinkdb.sum)
- description and source-code
```javascript
sum = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Sum, [{}].concat(slice.call(args.map(funcWrap))), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.sunday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>sunday {{signature}}](#apidoc.element.rethinkdb.sunday)
- description and source-code
```javascript
r.sunday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.table"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>table ()](#apidoc.element.rethinkdb.table)
- description and source-code
```javascript
table = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.tableCreate"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>tableCreate ()](#apidoc.element.rethinkdb.tableCreate)
- description and source-code
```javascript
tableCreate = function () {
  var args, expectedPosArgs, numPosArgs, perhapsOptDict;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  expectedPosArgs = fun.length - 1;
  perhapsOptDict = args[expectedPosArgs];
  if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
    perhapsOptDict = null;
  }
  numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
  if (expectedPosArgs !== numPosArgs) {
    if (expectedPosArgs !== 1) {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
    } else {
      throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
    }
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.tableDrop"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>tableDrop ()](#apidoc.element.rethinkdb.tableDrop)
- description and source-code
```javascript
tableDrop = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(TableDrop, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.tableList"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>tableList ()](#apidoc.element.rethinkdb.tableList)
- description and source-code
```javascript
tableList = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(TableList, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.thursday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>thursday {{signature}}](#apidoc.element.rethinkdb.thursday)
- description and source-code
```javascript
r.thursday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.time"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>time ()](#apidoc.element.rethinkdb.time)
- description and source-code
```javascript
time = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Time, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.tuesday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>tuesday {{signature}}](#apidoc.element.rethinkdb.tuesday)
- description and source-code
```javascript
r.tuesday
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.typeOf"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>typeOf ()](#apidoc.element.rethinkdb.typeOf)
- description and source-code
```javascript
typeOf = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(TypeOf, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.union"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>union ()](#apidoc.element.rethinkdb.union)
- description and source-code
```javascript
union = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(Union, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.uuid"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>uuid ()](#apidoc.element.rethinkdb.uuid)
- description and source-code
```javascript
uuid = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  return (function(func, args, ctor) {
    ctor.prototype = func.prototype;
    var child = new ctor, result = func.apply(child, args);
    return Object(result) === result ? result : child;
  })(UUID, [{}].concat(slice.call(args)), function(){});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.wednesday"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>wednesday {{signature}}](#apidoc.element.rethinkdb.wednesday)
- description and source-code
```javascript
r.wednesday
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error"></a>[module rethinkdb.Error](#apidoc.module.rethinkdb.Error)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAuthError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError)
- description and source-code
```javascript
function ReqlAuthError() {
  return ReqlAuthError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlAvailabilityError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError)
- description and source-code
```javascript
function ReqlAvailabilityError() {
  return ReqlAvailabilityError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError)
- description and source-code
```javascript
function ReqlCompileError() {
  return ReqlCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError)
- description and source-code
```javascript
function ReqlDriverCompileError() {
  return ReqlDriverCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
...
IterableResult.prototype._each = IterableResult.prototype.each;

IterableResult.prototype._eachAsync = IterableResult.prototype.eachAsync;

IterableResult.prototype.toArray = varar(0, 1, function(cb) {
  var results, wrapper;
  if ((cb != null) && typeof cb !== 'function') {
    throw new error.ReqlDriverCompileError("First argument to 'toArray' must be a function or undefined.");
  }
  results = [];
  wrapper = (function(_this) {
    return function(res) {
      results.push(res);
      return void 0;
    };
...
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverError ()](#apidoc.element.rethinkdb.Error.ReqlDriverError)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
...
  return this._responses.length === 0 || this._responses[0].r.length <= this._responseIndex;
};

IterableResult.prototype._promptNext = function() {
  var cb, errType, response;
  if (this._closeCbPromise != null) {
    cb = this._getCallback();
    cb(new error.ReqlDriverError("Cursor is closed."));
  }
  while (this._cbQueue[0] != null) {
    if (this.bufferEmpty() === true) {
      if (this._endFlag === true) {
        cb = this._getCallback();
        cb(new error.ReqlDriverError("No more rows in the cursor."));
      } else if (this._responses.length <= 1) {
...
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError)
- description and source-code
```javascript
function ReqlError(msg, term, frames) {
  this.name = this.constructor.name;
  this.msg = msg;
  this.frames = frames != null ? frames.slice(0) : void 0;
  if (term != null) {
    if (msg[msg.length - 1] === '.') {
      this.message = (msg.slice(0, msg.length - 1)) + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter
.prototype.printCarrots(term, frames));
    } else {
      this.message = msg + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter.prototype.printCarrots
(term, frames));
    }
  } else {
    this.message = "" + msg;
  }
  if (Error.captureStackTrace != null) {
    Error.captureStackTrace(this, this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlInternalError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError)
- description and source-code
```javascript
function ReqlInternalError() {
  return ReqlInternalError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlNonExistenceError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError)
- description and source-code
```javascript
function ReqlNonExistenceError() {
  return ReqlNonExistenceError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpFailedError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError)
- description and source-code
```javascript
function ReqlOpFailedError() {
  return ReqlOpFailedError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError)
- description and source-code
```javascript
function ReqlOpIndeterminateError() {
  return ReqlOpIndeterminateError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlPermissionError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError)
- description and source-code
```javascript
function ReqlPermissionError() {
  return ReqlPermissionError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlQueryLogicError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError)
- description and source-code
```javascript
function ReqlQueryLogicError() {
  return ReqlQueryLogicError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlResourceLimitError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError)
- description and source-code
```javascript
function ReqlResourceLimitError() {
  return ReqlResourceLimitError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlRuntimeError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlServerCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError)
- description and source-code
```javascript
function ReqlServerCompileError() {
  return ReqlServerCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlTimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError)
- description and source-code
```javascript
function ReqlTimeoutError() {
  return ReqlTimeoutError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlUserError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError)
- description and source-code
```javascript
function ReqlUserError() {
  return ReqlUserError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlClientError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlCompileError ()](#apidoc.element.rethinkdb.Error.RqlCompileError)
- description and source-code
```javascript
function ReqlCompileError() {
  return ReqlCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlDriverError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlDriverError ()](#apidoc.element.rethinkdb.Error.RqlDriverError)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlRuntimeError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlRuntimeError ()](#apidoc.element.rethinkdb.Error.RqlRuntimeError)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlServerError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlServerError ()](#apidoc.element.rethinkdb.Error.RqlServerError)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.printQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>printQuery (term)](#apidoc.element.rethinkdb.Error.printQuery)
- description and source-code
```javascript
printQuery = function (term) {
  var tree;
  tree = composeTerm(term);
  return joinTree(tree);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlAuthError"></a>[module rethinkdb.Error.ReqlAuthError](#apidoc.module.rethinkdb.Error.ReqlAuthError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAuthError.ReqlAuthError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAuthError ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.ReqlAuthError)
- description and source-code
```javascript
function ReqlAuthError() {
  return ReqlAuthError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlAuthError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlAuthError.prototype"></a>[module rethinkdb.Error.ReqlAuthError.prototype](#apidoc.module.rethinkdb.Error.ReqlAuthError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAuthError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAuthError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlAuthError.prototype.constructor)
- description and source-code
```javascript
function ReqlAuthError() {
  return ReqlAuthError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlAvailabilityError"></a>[module rethinkdb.Error.ReqlAvailabilityError](#apidoc.module.rethinkdb.Error.ReqlAvailabilityError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAvailabilityError.ReqlAvailabilityError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlAvailabilityError ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.ReqlAvailabilityError)
- description and source-code
```javascript
function ReqlAvailabilityError() {
  return ReqlAvailabilityError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlAvailabilityError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlAvailabilityError.prototype"></a>[module rethinkdb.Error.ReqlAvailabilityError.prototype](#apidoc.module.rethinkdb.Error.ReqlAvailabilityError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlAvailabilityError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlAvailabilityError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlAvailabilityError.prototype.constructor)
- description and source-code
```javascript
function ReqlAvailabilityError() {
  return ReqlAvailabilityError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlCompileError"></a>[module rethinkdb.Error.ReqlCompileError](#apidoc.module.rethinkdb.Error.ReqlCompileError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlCompileError.ReqlCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlCompileError ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.ReqlCompileError)
- description and source-code
```javascript
function ReqlCompileError() {
  return ReqlCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlCompileError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlCompileError.prototype"></a>[module rethinkdb.Error.ReqlCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlCompileError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlCompileError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlCompileError.prototype.constructor)
- description and source-code
```javascript
function ReqlCompileError() {
  return ReqlCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlDriverCompileError"></a>[module rethinkdb.Error.ReqlDriverCompileError](#apidoc.module.rethinkdb.Error.ReqlDriverCompileError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverCompileError.ReqlDriverCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlDriverCompileError ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.ReqlDriverCompileError)
- description and source-code
```javascript
function ReqlDriverCompileError() {
  return ReqlDriverCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
...
IterableResult.prototype._each = IterableResult.prototype.each;

IterableResult.prototype._eachAsync = IterableResult.prototype.eachAsync;

IterableResult.prototype.toArray = varar(0, 1, function(cb) {
  var results, wrapper;
  if ((cb != null) && typeof cb !== 'function') {
    throw new error.ReqlDriverCompileError("First argument to 'toArray' must be a function or undefined.");
  }
  results = [];
  wrapper = (function(_this) {
    return function(res) {
      results.push(res);
      return void 0;
    };
...
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverCompileError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlDriverCompileError.prototype"></a>[module rethinkdb.Error.ReqlDriverCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlDriverCompileError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlDriverCompileError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlDriverCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlDriverCompileError.prototype.constructor)
- description and source-code
```javascript
function ReqlDriverCompileError() {
  return ReqlDriverCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlError"></a>[module rethinkdb.Error.ReqlError](#apidoc.module.rethinkdb.Error.ReqlError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlError.ReqlError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlError (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError.ReqlError)
- description and source-code
```javascript
function ReqlError(msg, term, frames) {
  this.name = this.constructor.name;
  this.msg = msg;
  this.frames = frames != null ? frames.slice(0) : void 0;
  if (term != null) {
    if (msg[msg.length - 1] === '.') {
      this.message = (msg.slice(0, msg.length - 1)) + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter
.prototype.printCarrots(term, frames));
    } else {
      this.message = msg + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter.prototype.printCarrots
(term, frames));
    }
  } else {
    this.message = "" + msg;
  }
  if (Error.captureStackTrace != null) {
    Error.captureStackTrace(this, this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlError.prototype"></a>[module rethinkdb.Error.ReqlError.prototype](#apidoc.module.rethinkdb.Error.ReqlError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlError.prototype.</span>constructor (msg, term, frames)](#apidoc.element.rethinkdb.Error.ReqlError.prototype.constructor)
- description and source-code
```javascript
function ReqlError(msg, term, frames) {
  this.name = this.constructor.name;
  this.msg = msg;
  this.frames = frames != null ? frames.slice(0) : void 0;
  if (term != null) {
    if (msg[msg.length - 1] === '.') {
      this.message = (msg.slice(0, msg.length - 1)) + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter
.prototype.printCarrots(term, frames));
    } else {
      this.message = msg + " in:\n" + (ReqlQueryPrinter.prototype.printQuery(term)) + "\n" + (ReqlQueryPrinter.prototype.printCarrots
(term, frames));
    }
  } else {
    this.message = "" + msg;
  }
  if (Error.captureStackTrace != null) {
    Error.captureStackTrace(this, this);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlInternalError"></a>[module rethinkdb.Error.ReqlInternalError](#apidoc.module.rethinkdb.Error.ReqlInternalError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlInternalError.ReqlInternalError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlInternalError ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.ReqlInternalError)
- description and source-code
```javascript
function ReqlInternalError() {
  return ReqlInternalError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlInternalError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlInternalError.prototype"></a>[module rethinkdb.Error.ReqlInternalError.prototype](#apidoc.module.rethinkdb.Error.ReqlInternalError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlInternalError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlInternalError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlInternalError.prototype.constructor)
- description and source-code
```javascript
function ReqlInternalError() {
  return ReqlInternalError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlNonExistenceError"></a>[module rethinkdb.Error.ReqlNonExistenceError](#apidoc.module.rethinkdb.Error.ReqlNonExistenceError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlNonExistenceError.ReqlNonExistenceError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlNonExistenceError ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.ReqlNonExistenceError)
- description and source-code
```javascript
function ReqlNonExistenceError() {
  return ReqlNonExistenceError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlNonExistenceError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlNonExistenceError.prototype"></a>[module rethinkdb.Error.ReqlNonExistenceError.prototype](#apidoc.module.rethinkdb.Error.ReqlNonExistenceError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlNonExistenceError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlNonExistenceError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlNonExistenceError.prototype.constructor)
- description and source-code
```javascript
function ReqlNonExistenceError() {
  return ReqlNonExistenceError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlOpFailedError"></a>[module rethinkdb.Error.ReqlOpFailedError](#apidoc.module.rethinkdb.Error.ReqlOpFailedError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpFailedError.ReqlOpFailedError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpFailedError ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.ReqlOpFailedError)
- description and source-code
```javascript
function ReqlOpFailedError() {
  return ReqlOpFailedError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpFailedError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlOpFailedError.prototype"></a>[module rethinkdb.Error.ReqlOpFailedError.prototype](#apidoc.module.rethinkdb.Error.ReqlOpFailedError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpFailedError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpFailedError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlOpFailedError.prototype.constructor)
- description and source-code
```javascript
function ReqlOpFailedError() {
  return ReqlOpFailedError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError"></a>[module rethinkdb.Error.ReqlOpIndeterminateError](#apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.ReqlOpIndeterminateError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlOpIndeterminateError ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.ReqlOpIndeterminateError)
- description and source-code
```javascript
function ReqlOpIndeterminateError() {
  return ReqlOpIndeterminateError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError.prototype"></a>[module rethinkdb.Error.ReqlOpIndeterminateError.prototype](#apidoc.module.rethinkdb.Error.ReqlOpIndeterminateError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlOpIndeterminateError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlOpIndeterminateError.prototype.constructor)
- description and source-code
```javascript
function ReqlOpIndeterminateError() {
  return ReqlOpIndeterminateError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlPermissionError"></a>[module rethinkdb.Error.ReqlPermissionError](#apidoc.module.rethinkdb.Error.ReqlPermissionError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlPermissionError.ReqlPermissionError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlPermissionError ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.ReqlPermissionError)
- description and source-code
```javascript
function ReqlPermissionError() {
  return ReqlPermissionError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlPermissionError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlPermissionError.prototype"></a>[module rethinkdb.Error.ReqlPermissionError.prototype](#apidoc.module.rethinkdb.Error.ReqlPermissionError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlPermissionError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlPermissionError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlPermissionError.prototype.constructor)
- description and source-code
```javascript
function ReqlPermissionError() {
  return ReqlPermissionError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlQueryLogicError"></a>[module rethinkdb.Error.ReqlQueryLogicError](#apidoc.module.rethinkdb.Error.ReqlQueryLogicError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlQueryLogicError.ReqlQueryLogicError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlQueryLogicError ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.ReqlQueryLogicError)
- description and source-code
```javascript
function ReqlQueryLogicError() {
  return ReqlQueryLogicError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlQueryLogicError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlQueryLogicError.prototype"></a>[module rethinkdb.Error.ReqlQueryLogicError.prototype](#apidoc.module.rethinkdb.Error.ReqlQueryLogicError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlQueryLogicError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlQueryLogicError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlQueryLogicError.prototype.constructor)
- description and source-code
```javascript
function ReqlQueryLogicError() {
  return ReqlQueryLogicError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlResourceLimitError"></a>[module rethinkdb.Error.ReqlResourceLimitError](#apidoc.module.rethinkdb.Error.ReqlResourceLimitError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlResourceLimitError.ReqlResourceLimitError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlResourceLimitError ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.ReqlResourceLimitError)
- description and source-code
```javascript
function ReqlResourceLimitError() {
  return ReqlResourceLimitError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlResourceLimitError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlResourceLimitError.prototype"></a>[module rethinkdb.Error.ReqlResourceLimitError.prototype](#apidoc.module.rethinkdb.Error.ReqlResourceLimitError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlResourceLimitError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlResourceLimitError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlResourceLimitError.prototype.constructor)
- description and source-code
```javascript
function ReqlResourceLimitError() {
  return ReqlResourceLimitError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlRuntimeError"></a>[module rethinkdb.Error.ReqlRuntimeError](#apidoc.module.rethinkdb.Error.ReqlRuntimeError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlRuntimeError.ReqlRuntimeError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlRuntimeError ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.ReqlRuntimeError)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlRuntimeError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlRuntimeError.prototype"></a>[module rethinkdb.Error.ReqlRuntimeError.prototype](#apidoc.module.rethinkdb.Error.ReqlRuntimeError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlRuntimeError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlRuntimeError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlRuntimeError.prototype.constructor)
- description and source-code
```javascript
function ReqlRuntimeError() {
  return ReqlRuntimeError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlServerCompileError"></a>[module rethinkdb.Error.ReqlServerCompileError](#apidoc.module.rethinkdb.Error.ReqlServerCompileError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlServerCompileError.ReqlServerCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlServerCompileError ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.ReqlServerCompileError)
- description and source-code
```javascript
function ReqlServerCompileError() {
  return ReqlServerCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlServerCompileError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlServerCompileError.prototype"></a>[module rethinkdb.Error.ReqlServerCompileError.prototype](#apidoc.module.rethinkdb.Error.ReqlServerCompileError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlServerCompileError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlServerCompileError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlServerCompileError.prototype.constructor)
- description and source-code
```javascript
function ReqlServerCompileError() {
  return ReqlServerCompileError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlTimeoutError"></a>[module rethinkdb.Error.ReqlTimeoutError](#apidoc.module.rethinkdb.Error.ReqlTimeoutError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlTimeoutError.ReqlTimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlTimeoutError ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.ReqlTimeoutError)
- description and source-code
```javascript
function ReqlTimeoutError() {
  return ReqlTimeoutError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlTimeoutError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlTimeoutError.prototype"></a>[module rethinkdb.Error.ReqlTimeoutError.prototype](#apidoc.module.rethinkdb.Error.ReqlTimeoutError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlTimeoutError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlTimeoutError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlTimeoutError.prototype.constructor)
- description and source-code
```javascript
function ReqlTimeoutError() {
  return ReqlTimeoutError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlUserError"></a>[module rethinkdb.Error.ReqlUserError](#apidoc.module.rethinkdb.Error.ReqlUserError)

#### <a name="apidoc.element.rethinkdb.Error.ReqlUserError.ReqlUserError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>ReqlUserError ()](#apidoc.element.rethinkdb.Error.ReqlUserError.ReqlUserError)
- description and source-code
```javascript
function ReqlUserError() {
  return ReqlUserError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.ReqlUserError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.ReqlUserError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.ReqlUserError.prototype"></a>[module rethinkdb.Error.ReqlUserError.prototype](#apidoc.module.rethinkdb.Error.ReqlUserError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.ReqlUserError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.ReqlUserError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.ReqlUserError.prototype.constructor)
- description and source-code
```javascript
function ReqlUserError() {
  return ReqlUserError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.RqlClientError"></a>[module rethinkdb.Error.RqlClientError](#apidoc.module.rethinkdb.Error.RqlClientError)

#### <a name="apidoc.element.rethinkdb.Error.RqlClientError.RqlClientError"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.</span>RqlClientError ()](#apidoc.element.rethinkdb.Error.RqlClientError.RqlClientError)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.Error.RqlClientError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.</span>captureStackTrace ()](#apidoc.element.rethinkdb.Error.RqlClientError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.Error.RqlClientError.prototype"></a>[module rethinkdb.Error.RqlClientError.prototype](#apidoc.module.rethinkdb.Error.RqlClientError.prototype)

#### <a name="apidoc.element.rethinkdb.Error.RqlClientError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.Error.RqlClientError.prototype.</span>constructor ()](#apidoc.element.rethinkdb.Error.RqlClientError.prototype.constructor)
- description and source-code
```javascript
function ReqlDriverError() {
  return ReqlDriverError.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird"></a>[module rethinkdb._bluebird](#apidoc.module.rethinkdb._bluebird)

#### <a name="apidoc.element.rethinkdb._bluebird._bluebird"></a>[function <span class="apidocSignatureSpan">rethinkdb.</span>_bluebird (resolver)](#apidoc.element.rethinkdb._bluebird._bluebird)
- description and source-code
```javascript
function Promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("the promise constructor requires a resolver function\u000a\u000a    See http://goo.gl/EC22Yn\u000a");
    }
    if (this.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/KsIlge\u000a");
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._progressHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._settledValue = undefined;
    if (resolver !== INTERNAL) this._resolveFromResolver(resolver);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.CancellationError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.OperationalError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.Promise"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>Promise (resolver)](#apidoc.element.rethinkdb._bluebird.Promise)
- description and source-code
```javascript
function Promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("the promise constructor requires a resolver function\u000a\u000a    See http://goo.gl/EC22Yn\u000a");
    }
    if (this.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/KsIlge\u000a");
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._progressHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._settledValue = undefined;
    if (resolver !== INTERNAL) this._resolveFromResolver(resolver);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValue = promise._settledValue;
    }
    else {
        this._bitField = 0;
        this._settledValue = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.RangeError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>RangeError ()](#apidoc.element.rethinkdb._bluebird.RangeError)
- description and source-code
```javascript
function RangeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.RejectionError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>RejectionError (message)](#apidoc.element.rethinkdb._bluebird.RejectionError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.TimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.TypeError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TypeError ()](#apidoc.element.rethinkdb._bluebird.TypeError)
- description and source-code
```javascript
function TypeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>_SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.all"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>all (promises)](#apidoc.element.rethinkdb._bluebird.all)
- description and source-code
```javascript
all = function (promises) {
    return new PromiseArray(promises).promise();
}
```
- example usage
```shell
...
          return pending.splice(pending.indexOf(p), 1);
        });
        return pending.push(p);
      }).then(nextCb)["catch"](function(err) {
        if ((err != null ? err.message : void 0) !== 'No more rows in the cursor.') {
          throw err;
        }
        return Promise.all(pending);
      });
    }
  };
})(this);
resPromise = nextCb().then(function() {
  if (errCb != null) {
    return errCb(null);
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.any"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>any (promises)](#apidoc.element.rethinkdb._bluebird.any)
- description and source-code
```javascript
any = function (promises) {
    return any(promises);
}
```
- example usage
```shell
...
    throw new error.ReqlDriverError("Cursor is closed.");
  });
} else {
  return _this._next().then(function(data) {
    if (pending.length < options.concurrency) {
      return data;
    }
    return Promise.any(pending)["catch"](Promise.AggregateError, function(errs) {
      throw errs[0];
    })["return"](data);
  }).then(function(data) {
    var p;
    p = userCb(data).then(function() {
      return pending.splice(pending.indexOf(p), 1);
    });
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.attempt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>attempt (fn, args, ctx)](#apidoc.element.rethinkdb._bluebird.attempt)
- description and source-code
```javascript
attempt = function (fn, args, ctx) {
    if (typeof fn !== "function") {
        return apiRejection("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value = util.isArray(args)
        ? tryCatch(fn).apply(ctx, args)
        : tryCatch(fn).call(ctx, args);
    ret._popContext();
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.bind"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>bind (thisArg, value)](#apidoc.element.rethinkdb._bluebird.bind)
- description and source-code
```javascript
bind = function (thisArg, value) {
    var maybePromise = tryConvertToPromise(thisArg);
    var ret = new Promise(INTERNAL);

    ret._setBoundTo(maybePromise);
    if (maybePromise instanceof Promise) {
        maybePromise._then(function() {
            ret._resolveCallback(value);
        }, ret._reject, ret._progress, ret, null);
    } else {
        ret._resolveCallback(value);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.cast"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>cast (obj)](#apidoc.element.rethinkdb._bluebird.cast)
- description and source-code
```javascript
cast = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        var val = ret;
        ret = new Promise(INTERNAL);
        ret._fulfillUnchecked(val);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.coroutine"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/6Vqhm0\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        spawn._generator = generator;
        spawn._next(undefined);
        return spawn.promise();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.defer"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>defer ()](#apidoc.element.rethinkdb._bluebird.defer)
- description and source-code
```javascript
defer = function () {
    var promise = new Promise(INTERNAL);
    return new PromiseResolver(promise);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.delay"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>delay (value, ms)](#apidoc.element.rethinkdb._bluebird.delay)
- description and source-code
```javascript
delay = function (value, ms) {
    if (ms === undefined) {
        ms = value;
        value = undefined;
        var ret = new Promise(INTERNAL);
        setTimeout(function() { ret._fulfill(); }, ms);
        return ret;
    }
    ms = +ms;
    return Promise.resolve(value)._then(afterValue, null, null, ms, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.each"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>each (promises, fn)](#apidoc.element.rethinkdb._bluebird.each)
- description and source-code
```javascript
each = function (promises, fn) {
    return PromiseReduce(promises, fn, null, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.filter"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>filter (promises, fn, options)](#apidoc.element.rethinkdb._bluebird.filter)
- description and source-code
```javascript
filter = function (promises, fn, options) {
    return PromiseMap(promises, fn, options, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.fromNode"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>fromNode (fn)](#apidoc.element.rethinkdb._bluebird.fromNode)
- description and source-code
```javascript
fromNode = function (fn) {
    var ret = new Promise(INTERNAL);
    var result = tryCatch(fn)(nodebackForPromise(ret));
    if (result === errorObj) {
        ret._rejectCallback(result.e, true, true);
    }
    return ret;
}
```
- example usage
```shell
...
  }
  fn = (function(_this) {
    return function(cb) {
      _this._cbQueue.push(cb);
      return _this._promptNext();
    };
  })(this);
  return Promise.fromNode(fn).nodeify(cb);
});

IterableResult.prototype.close = varar(0, 1, function(cb) {
  if (this._closeCbPromise != null) {
    if (this._closeCbPromise.isPending()) {
      this._closeCbPromise = this._closeCbPromise.nodeify(cb);
    } else {
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.fulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>fulfilled (obj)](#apidoc.element.rethinkdb._bluebird.fulfilled)
- description and source-code
```javascript
fulfilled = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        var val = ret;
        ret = new Promise(INTERNAL);
        ret._fulfillUnchecked(val);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.getNewLibraryCopy"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>getNewLibraryCopy ()](#apidoc.element.rethinkdb._bluebird.getNewLibraryCopy)
- description and source-code
```javascript
getNewLibraryCopy = function () {
var makeSelfResolutionError = function () {
    return new TypeError("circular promise resolution chain\u000a\u000a    See http://goo.gl/LhFpo0\u000a");
};
var reflect = function() {
    return new Promise.PromiseInspection(this._target());
};
var apiRejection = function(msg) {
    return Promise.reject(new TypeError(msg));
};

var util = require("./util.js");

var getDomain;
if (util.isNode) {
    getDomain = function() {
        var ret = process.domain;
        if (ret === undefined) ret = null;
        return ret;
    };
} else {
    getDomain = function() {
        return null;
    };
}
util.notEnumerableProp(Promise, "_getDomain", getDomain);

var UNDEFINED_BINDING = {};
var async = require("./async.js");
var errors = require("./errors.js");
var TypeError = Promise.TypeError = errors.TypeError;
Promise.RangeError = errors.RangeError;
Promise.CancellationError = errors.CancellationError;
Promise.TimeoutError = errors.TimeoutError;
Promise.OperationalError = errors.OperationalError;
Promise.RejectionError = errors.OperationalError;
Promise.AggregateError = errors.AggregateError;
var INTERNAL = function(){};
var APPLY = {};
var NEXT_FILTER = {e: null};
var tryConvertToPromise = require("./thenables.js")(Promise, INTERNAL);
var PromiseArray =
    require("./promise_array.js")(Promise, INTERNAL,
                                    tryConvertToPromise, apiRejection);
var CapturedTrace = require("./captured_trace.js")();
var isDebugging = require("./debuggability.js")(Promise, CapturedTrace);
<span class="apidocCodeCommentSpan"> /*jshint unused:false*/
</span>var createContext =
    require("./context.js")(Promise, CapturedTrace, isDebugging);
var CatchFilter = require("./catch_filter.js")(NEXT_FILTER);
var PromiseResolver = require("./promise_resolver.js");
var nodebackForPromise = PromiseResolver._nodebackForPromise;
var errorObj = util.errorObj;
var tryCatch = util.tryCatch;

function Promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("the promise constructor requires a resolver function\u000a\u000a    See http://goo.gl/EC22Yn\u000a");
    }
    if (this.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/KsIlge\u000a");
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._progressHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._settledValue = undefined;
    if (resolver !== INTERNAL) this._resolveFromResolver(resolver);
}

Promise.prototype.toString = function () {
    return "[object Promise]";
};

Promise.prototype.caught = Promise.prototype["catch"] = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (typeof item === "function") {
                catchInstances[j++] = item;
            } else {
                return Promise.reject(
                    new TypeError("Catch filter must inherit from Error or be a simple predicate function\u000a\u000a    See http
://goo.gl/o84o68\u000a"));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        var catchFilter = new CatchFilter(catchInstances, fn, this);
        return this._then(undefined, catchFilter.doFilter, undefined,
            catchFilter, undefined);
    }
    return this._then(undefined, fn, undefined, undefined, undefined);
};

Promise.prototype.reflect = function () {
    return this._then(reflect, reflect, undefined, this, undefined);
};

Promise.prototype.then = function (didFulfill, didReject, didProgress) {
    if (isDebugging() && arguments.length > 0 &&
        typeof didFulfill !== "function" &&
        typeof didReject !== "function") {
        var msg = ".then() only accepts functions but was passed: " +
                util.classString(didFulfill);
        if (arguments.length > 1) {
            msg += ", " + util.class ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.hasLongStackTraces"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>hasLongStackTraces ()](#apidoc.element.rethinkdb._bluebird.hasLongStackTraces)
- description and source-code
```javascript
hasLongStackTraces = function () {
    return debugging && CapturedTrace.isSupported();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.is"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>is (val)](#apidoc.element.rethinkdb._bluebird.is)
- description and source-code
```javascript
is = function (val) {
    return val instanceof Promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.join"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>join ()](#apidoc.element.rethinkdb._bluebird.join)
- description and source-code
```javascript
join = function () {
    var last = arguments.length - 1;
    var fn;
    if (last > 0 && typeof arguments[last] === "function") {
        fn = arguments[last];
        if (!false) {
            if (last < 6 && canEvaluate) {
                var ret = new Promise(INTERNAL);
                ret._captureStackTrace();
                var holder = new Holder(last, fn);
                var callbacks = thenCallbacks;
                for (var i = 0; i < last; ++i) {
                    var maybePromise = tryConvertToPromise(arguments[i], ret);
                    if (maybePromise instanceof Promise) {
                        maybePromise = maybePromise._target();
                        if (maybePromise._isPending()) {
                            maybePromise._then(callbacks[i], reject,
                                               undefined, ret, holder);
                        } else if (maybePromise._isFulfilled()) {
                            callbacks[i].call(ret,
                                              maybePromise._value(), holder);
                        } else {
                            ret._reject(maybePromise._reason());
                        }
                    } else {
                        callbacks[i].call(ret, maybePromise, holder);
                    }
                }
                return ret;
            }
        }
    }
    var $_len = arguments.length;var args = new Array($_len); for(var $_i = 0; $_i < $_len; ++$_i) {args[$_i] = arguments[$_i];}
    if (fn) args.pop();
    var ret = new PromiseArray(args).promise();
    return fn !== undefined ? ret.spread(fn) : ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.longStackTraces"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>longStackTraces ()](#apidoc.element.rethinkdb._bluebird.longStackTraces)
- description and source-code
```javascript
longStackTraces = function () {
    if (async.haveItemsQueued() &&
        debugging === false
   ) {
        throw new Error("cannot enable long stack traces after promises have been created\u000a\u000a    See http://goo.gl/DT1qyG\u000a");
    }
    debugging = CapturedTrace.isSupported();
    if (debugging) {
        async.disableTrampolineIfNecessary();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.map"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>map (promises, fn, options, _filter)](#apidoc.element.rethinkdb._bluebird.map)
- description and source-code
```javascript
map = function (promises, fn, options, _filter) {
    if (typeof fn !== "function") return apiRejection("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    return map(promises, fn, options, _filter).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.method"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>method (fn)](#apidoc.element.rethinkdb._bluebird.method)
- description and source-code
```javascript
method = function (fn) {
    if (typeof fn !== "function") {
        throw new Promise.TypeError("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    }
    return function () {
        var ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._pushContext();
        var value = tryCatch(fn).apply(this, arguments);
        ret._popContext();
        ret._resolveFromSyncValue(value);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.noConflict"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>noConflict ()](#apidoc.element.rethinkdb._bluebird.noConflict)
- description and source-code
```javascript
function noConflict() {
    try { if (Promise === bluebird) Promise = old; }
    catch (e) {}
    return bluebird;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.onPossiblyUnhandledRejection"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.rethinkdb._bluebird.onPossiblyUnhandledRejection)
- description and source-code
```javascript
onPossiblyUnhandledRejection = function (fn) {
    var domain = getDomain();
    possiblyUnhandledRejection =
        typeof fn === "function" ? (domain === null ? fn : domain.bind(fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.onUnhandledRejectionHandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.rethinkdb._bluebird.onUnhandledRejectionHandled)
- description and source-code
```javascript
onUnhandledRejectionHandled = function (fn) {
    var domain = getDomain();
    unhandledRejectionHandled =
        typeof fn === "function" ? (domain === null ? fn : domain.bind(fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.pending"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>pending ()](#apidoc.element.rethinkdb._bluebird.pending)
- description and source-code
```javascript
pending = function () {
    var promise = new Promise(INTERNAL);
    return new PromiseResolver(promise);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.promisify"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>promisify (fn, receiver)](#apidoc.element.rethinkdb._bluebird.promisify)
- description and source-code
```javascript
promisify = function (fn, receiver) {
    if (typeof fn !== "function") {
        throw new TypeError("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    }
    if (isPromisified(fn)) {
        return fn;
    }
    var ret = promisify(fn, arguments.length < 2 ? THIS : receiver);
    util.copyDescriptors(fn, ret, propsFilter);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.promisifyAll"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>promisifyAll (target, options)](#apidoc.element.rethinkdb._bluebird.promisifyAll)
- description and source-code
```javascript
promisifyAll = function (target, options) {
    if (typeof target !== "function" && typeof target !== "object") {
        throw new TypeError("the target of promisifyAll must be an object or a function\u000a\u000a    See http://goo.gl/9ITlV0\
u000a");
    }
    options = Object(options);
    var suffix = options.suffix;
    if (typeof suffix !== "string") suffix = defaultSuffix;
    var filter = options.filter;
    if (typeof filter !== "function") filter = defaultFilter;
    var promisifier = options.promisifier;
    if (typeof promisifier !== "function") promisifier = makeNodePromisified;

    if (!util.isIdentifier(suffix)) {
        throw new RangeError("suffix must be a valid identifier\u000a\u000a    See http://goo.gl/8FZo5V\u000a");
    }

    var keys = util.inheritedDataKeys(target);
    for (var i = 0; i < keys.length; ++i) {
        var value = target[keys[i]];
        if (keys[i] !== "constructor" &&
            util.isClass(value)) {
            promisifyAll(value.prototype, suffix, filter, promisifier);
            promisifyAll(value, suffix, filter, promisifier);
        }
    }

    return promisifyAll(target, suffix, filter, promisifier);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.props"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>props (promises)](#apidoc.element.rethinkdb._bluebird.props)
- description and source-code
```javascript
props = function (promises) {
    return props(promises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.race"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>race (promises)](#apidoc.element.rethinkdb._bluebird.race)
- description and source-code
```javascript
race = function (promises) {
    return race(promises, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.reduce"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.rethinkdb._bluebird.reduce)
- description and source-code
```javascript
reduce = function (promises, fn, initialValue, _each) {
    return reduce(promises, fn, initialValue, _each);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.reject"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>reject (reason)](#apidoc.element.rethinkdb._bluebird.reject)
- description and source-code
```javascript
reject = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.rejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>rejected (reason)](#apidoc.element.rethinkdb._bluebird.rejected)
- description and source-code
```javascript
rejected = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.resolve"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>resolve (obj)](#apidoc.element.rethinkdb._bluebird.resolve)
- description and source-code
```javascript
resolve = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        var val = ret;
        ret = new Promise(INTERNAL);
        ret._fulfillUnchecked(val);
    }
    return ret;
}
```
- example usage
```shell
...
});

IterableResult.prototype.close = varar(0, 1, function(cb) {
  if (this._closeCbPromise != null) {
    if (this._closeCbPromise.isPending()) {
      this._closeCbPromise = this._closeCbPromise.nodeify(cb);
    } else {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
    }
  } else {
    if (this._endFlag) {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
      this._responses = [];
      this._responseIndex = 0;
    } else {
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.setScheduler"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>setScheduler (fn)](#apidoc.element.rethinkdb._bluebird.setScheduler)
- description and source-code
```javascript
setScheduler = function (fn) {
    if (typeof fn !== "function") throw new TypeError("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    var prev = async._schedule;
    async._schedule = fn;
    return prev;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.settle"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>settle (promises)](#apidoc.element.rethinkdb._bluebird.settle)
- description and source-code
```javascript
settle = function (promises) {
    return new SettledPromiseArray(promises).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.some"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>some (promises, howMany)](#apidoc.element.rethinkdb._bluebird.some)
- description and source-code
```javascript
some = function (promises, howMany) {
    return some(promises, howMany);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.spawn"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>spawn (generatorFunction)](#apidoc.element.rethinkdb._bluebird.spawn)
- description and source-code
```javascript
spawn = function (generatorFunction) {
    if (typeof generatorFunction !== "function") {
        return apiRejection("generatorFunction must be a function\u000a\u000a    See http://goo.gl/6Vqhm0\u000a");
    }
    var spawn = new PromiseSpawn(generatorFunction, this);
    var ret = spawn.promise();
    spawn._run(Promise.spawn);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.try"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>try (fn, args, ctx)](#apidoc.element.rethinkdb._bluebird.try)
- description and source-code
```javascript
try = function (fn, args, ctx) {
    if (typeof fn !== "function") {
        return apiRejection("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value = util.isArray(args)
        ? tryCatch(fn).apply(ctx, args)
        : tryCatch(fn).call(ctx, args);
    ret._popContext();
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.using"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>using ()](#apidoc.element.rethinkdb._bluebird.using)
- description and source-code
```javascript
using = function () {
    var len = arguments.length;
    if (len < 2) return apiRejection(
                    "you must pass at least 2 arguments to Promise.using");
    var fn = arguments[len - 1];
    if (typeof fn !== "function") return apiRejection("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");

    var input;
    var spreadArgs = true;
    if (len === 2 && Array.isArray(arguments[0])) {
        input = arguments[0];
        len = input.length;
        spreadArgs = false;
    } else {
        input = arguments;
        len--;
    }
    var resources = new Array(len);
    for (var i = 0; i < len; ++i) {
        var resource = input[i];
        if (Disposer.isDisposer(resource)) {
            var disposer = resource;
            resource = resource.promise();
            resource._setDisposable(disposer);
        } else {
            var maybePromise = tryConvertToPromise(resource);
            if (maybePromise instanceof Promise) {
                resource =
                    maybePromise._then(maybeUnwrapDisposer, null, null, {
                        resources: resources,
                        index: i
                }, undefined);
            }
        }
        resources[i] = resource;
    }

    var promise = Promise.settle(resources)
        .then(inspectionMapper)
        .then(function(vals) {
            promise._pushContext();
            var ret;
            try {
                ret = spreadArgs
                    ? fn.apply(undefined, vals) : fn.call(undefined,  vals);
            } finally {
                promise._popContext();
            }
            return ret;
        })
        ._then(
            disposerSuccess, disposerFail, undefined, resources, undefined);
    resources.promise = promise;
    return promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.AggregateError"></a>[module rethinkdb._bluebird.AggregateError](#apidoc.module.rethinkdb._bluebird.AggregateError)

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.AggregateError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>AggregateError (message)](#apidoc.element.rethinkdb._bluebird.AggregateError.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.AggregateError.prototype"></a>[module rethinkdb._bluebird.AggregateError.prototype](#apidoc.module.rethinkdb._bluebird.AggregateError.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.every"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>every ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.every)
- description and source-code
```javascript
function every() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.filter"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>filter ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.filter)
- description and source-code
```javascript
function filter() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.forEach"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>forEach ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.forEach)
- description and source-code
```javascript
function forEach() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>indexOf ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.indexOf)
- description and source-code
```javascript
function indexOf() { [native code] }
```
- example usage
```shell
...
  }
  return Promise.any(pending)["catch"](Promise.AggregateError, function(errs) {
    throw errs[0];
  })["return"](data);
}).then(function(data) {
  var p;
  p = userCb(data).then(function() {
    return pending.splice(pending.indexOf(p), 1);
  });
  return pending.push(p);
}).then(nextCb)["catch"](function(err) {
  if ((err != null ? err.message : void 0) !== 'No more rows in the cursor.') {
    throw err;
  }
  return Promise.all(pending);
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.join"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>join ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.map"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>map ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.map)
- description and source-code
```javascript
function map() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.pop"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>pop ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.pop)
- description and source-code
```javascript
function pop() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.push"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>push ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.push)
- description and source-code
```javascript
function push() { [native code] }
```
- example usage
```shell
...
  this._closeCbPromise = null;
  this.next = this._next;
}

IterableResult.prototype._addResponse = function(response) {
  if (response.t === this._type || response.t === protoResponseType.SUCCESS_SEQUENCE) {
    if (response.r.length > 0) {
      this._responses.push(response);
    }
  } else {
    this._responses.push(response);
  }
  this._outstandingRequests -= 1;
  if (response.t !== this._type) {
    this._endFlag = true;
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduce"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reduce ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduce)
- description and source-code
```javascript
function reduce() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reduceRight)
- description and source-code
```javascript
function reduceRight() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reverse"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>reverse ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.reverse)
- description and source-code
```javascript
function reverse() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.shift"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>shift ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.shift)
- description and source-code
```javascript
function shift() { [native code] }
```
- example usage
```shell
...
  }
  return this;
};

IterableResult.prototype._getCallback = function() {
  var cb, immediateCb;
  this._iterations += 1;
  cb = this._cbQueue.shift();
  if (this._iterations % this.stackSize === this.stackSize - 1) {
    immediateCb = (function(err, row) {
      return setImmediate(function() {
        return cb(err, row);
      });
    });
    return immediateCb;
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.slice"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>slice ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
...
  var fn;
  fn = (function(_this) {
    return function(cb) {
      if (_this._closeCbPromise != null) {
        cb(new error.ReqlDriverError("Cursor is closed."));
      }
      if (_this.__index != null) {
        return cb(null, _this.slice(_this.__index, _this.length));
      } else {
        return cb(null, _this);
      }
    };
  })(this);
  return Promise.fromNode(fn).nodeify(cb);
});
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.some"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>some ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.sort"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>sort ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.toString"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>toString ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var indent = Array(level * 4 + 1).join(" ");
    var ret = "\n" + indent + "AggregateError of:" + "\n";
    level++;
    indent = Array(level * 4 + 1).join(" ");
    for (var i = 0; i < this.length; ++i) {
        var str = this[i] === this ? "[Circular AggregateError]" : this[i] + "";
        var lines = str.split("\n");
        for (var j = 0; j < lines.length; ++j) {
            lines[j] = indent + lines[j];
        }
        str = lines.join("\n");
        ret += str + "\n";
    }
    level--;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.AggregateError.prototype.unshift"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.AggregateError.prototype.</span>unshift ()](#apidoc.element.rethinkdb._bluebird.AggregateError.prototype.unshift)
- description and source-code
```javascript
function unshift() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.CancellationError"></a>[module rethinkdb._bluebird.CancellationError](#apidoc.module.rethinkdb._bluebird.CancellationError)

#### <a name="apidoc.element.rethinkdb._bluebird.CancellationError.CancellationError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>CancellationError (message)](#apidoc.element.rethinkdb._bluebird.CancellationError.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.CancellationError.prototype"></a>[module rethinkdb._bluebird.CancellationError.prototype](#apidoc.module.rethinkdb._bluebird.CancellationError.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.CancellationError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.CancellationError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.CancellationError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.OperationalError"></a>[module rethinkdb._bluebird.OperationalError](#apidoc.module.rethinkdb._bluebird.OperationalError)

#### <a name="apidoc.element.rethinkdb._bluebird.OperationalError.OperationalError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>OperationalError (message)](#apidoc.element.rethinkdb._bluebird.OperationalError.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.OperationalError.prototype"></a>[module rethinkdb._bluebird.OperationalError.prototype](#apidoc.module.rethinkdb._bluebird.OperationalError.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.OperationalError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.OperationalError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.OperationalError.prototype.constructor)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.PromiseInspection"></a>[module rethinkdb._bluebird.PromiseInspection](#apidoc.module.rethinkdb._bluebird.PromiseInspection)

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.PromiseInspection"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>PromiseInspection (promise)](#apidoc.element.rethinkdb._bluebird.PromiseInspection.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValue = promise._settledValue;
    }
    else {
        this._bitField = 0;
        this._settledValue = undefined;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.PromiseInspection.prototype"></a>[module rethinkdb._bluebird.PromiseInspection.prototype](#apidoc.module.rethinkdb._bluebird.PromiseInspection.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.error"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>error ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.error)
- description and source-code
```javascript
error = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/hPuiwB\u000a
");
    }
    return this._settledValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return (this._bitField & 268435456) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isPending"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return (this._bitField & 402653184) === 0;
}
```
- example usage
```shell
...
    };
  })(this);
  return Promise.fromNode(fn).nodeify(cb);
});

IterableResult.prototype.close = varar(0, 1, function(cb) {
  if (this._closeCbPromise != null) {
    if (this._closeCbPromise.isPending()) {
      this._closeCbPromise = this._closeCbPromise.nodeify(cb);
    } else {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
    }
  } else {
    if (this._endFlag) {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return (this._bitField & 134217728) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isResolved"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.isResolved)
- description and source-code
```javascript
isResolved = function () {
    return (this._bitField & 402653184) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.reason"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>reason ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.reason)
- description and source-code
```javascript
reason = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/hPuiwB\u000a
");
    }
    return this._settledValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.value"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.PromiseInspection.prototype.</span>value ()](#apidoc.element.rethinkdb._bluebird.PromiseInspection.prototype.value)
- description and source-code
```javascript
value = function () {
    if (!this.isFulfilled()) {
        throw new TypeError("cannot get fulfillment value of a non-fulfilled promise\u000a\u000a    See http://goo.gl/hc1DLj\u000a
");
    }
    return this._settledValue;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.TimeoutError"></a>[module rethinkdb._bluebird.TimeoutError](#apidoc.module.rethinkdb._bluebird.TimeoutError)

#### <a name="apidoc.element.rethinkdb._bluebird.TimeoutError.TimeoutError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>TimeoutError (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.TimeoutError.prototype"></a>[module rethinkdb._bluebird.TimeoutError.prototype](#apidoc.module.rethinkdb._bluebird.TimeoutError.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.TimeoutError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.rethinkdb._bluebird.TimeoutError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird._SomePromiseArray"></a>[module rethinkdb._bluebird._SomePromiseArray](#apidoc.module.rethinkdb._bluebird._SomePromiseArray)

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>_SomePromiseArray (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird._SomePromiseArray.prototype"></a>[module rethinkdb._bluebird._SomePromiseArray.prototype](#apidoc.module.rethinkdb._bluebird._SomePromiseArray.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addFulfilled)
- description and source-code
```javascript
_addFulfilled = function (value) {
    this._values[this._totalResolved++] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._addRejected)
- description and source-code
```javascript
_addRejected = function (reason) {
    this._values.push(reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._canPossiblyFulfill"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._canPossiblyFulfill)
- description and source-code
```javascript
_canPossiblyFulfill = function () {
    return this.length() - this._rejected();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._fulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._fulfilled)
- description and source-code
```javascript
_fulfilled = function () {
    return this._totalResolved;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._getRangeError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._getRangeError)
- description and source-code
```javascript
_getRangeError = function (count) {
    var message = "Input array must contain at least " +
            this._howMany + " items but contains only " + count + " items";
    return new RangeError(message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._init"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._init)
- description and source-code
```javascript
_init = function () {
    if (!this._initialized) {
        return;
    }
    if (this._howMany === 0) {
        this._resolve([]);
        return;
    }
    this._init$(undefined, -5);
    var isArrayResolved = isArray(this._values);
    if (!this._isResolved() &&
        isArrayResolved &&
        this._howMany > this._canPossiblyFulfill()) {
        this._reject(this._getRangeError(this.length()));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseFulfilled)
- description and source-code
```javascript
_promiseFulfilled = function (value) {
    this._addFulfilled(value);
    if (this._fulfilled() === this.howMany()) {
        this._values.length = this.howMany();
        if (this.howMany() === 1 && this._unwrap) {
            this._resolve(this._values[0]);
        } else {
            this._resolve(this._values);
        }
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._promiseRejected)
- description and source-code
```javascript
_promiseRejected = function (reason) {
    this._addRejected(reason);
    if (this.howMany() > this._canPossiblyFulfill()) {
        var e = new AggregateError();
        for (var i = this.length(); i < this._values.length; ++i) {
            e.push(this._values[i]);
        }
        this._reject(e);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._rejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._rejected)
- description and source-code
```javascript
_rejected = function () {
    return this._values.length - this.length();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._resolveEmptyArray"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype._resolveEmptyArray)
- description and source-code
```javascript
_resolveEmptyArray = function () {
    this._reject(this._getRangeError(0));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.constructor)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.howMany"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.howMany)
- description and source-code
```javascript
howMany = function () {
    return this._howMany;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.init"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>init ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.init)
- description and source-code
```javascript
init = function () {
    this._initialized = true;
    this._init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setHowMany"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setHowMany)
- description and source-code
```javascript
setHowMany = function (count) {
    this._howMany = count;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setUnwrap"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.rethinkdb._bluebird._SomePromiseArray.prototype.setUnwrap)
- description and source-code
```javascript
setUnwrap = function () {
    this._unwrap = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.coroutine"></a>[module rethinkdb._bluebird.coroutine](#apidoc.module.rethinkdb._bluebird.coroutine)

#### <a name="apidoc.element.rethinkdb._bluebird.coroutine.coroutine"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.rethinkdb._bluebird.coroutine.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/6Vqhm0\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        spawn._generator = generator;
        spawn._next(undefined);
        return spawn.promise();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.coroutine.addYieldHandler"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.coroutine.</span>addYieldHandler (fn)](#apidoc.element.rethinkdb._bluebird.coroutine.addYieldHandler)
- description and source-code
```javascript
addYieldHandler = function (fn) {
    if (typeof fn !== "function") throw new TypeError("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");
    yieldHandlers.push(fn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb._bluebird.prototype"></a>[module rethinkdb._bluebird.prototype](#apidoc.module.rethinkdb._bluebird.prototype)

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._addCallbacks"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_addCallbacks ( fulfill, reject, progress, promise, receiver, domain )](#apidoc.element.rethinkdb._bluebird.prototype._addCallbacks)
- description and source-code
```javascript
_addCallbacks = function ( fulfill, reject, progress, promise, receiver, domain ) {
    var index = this._length();

    if (index >= 131071 - 5) {
        index = 0;
        this._setLength(0);
    }

    if (index === 0) {
        this._promise0 = promise;
        if (receiver !== undefined) this._receiver0 = receiver;
        if (typeof fulfill === "function" && !this._isCarryingStackTrace()) {
            this._fulfillmentHandler0 =
                domain === null ? fulfill : domain.bind(fulfill);
        }
        if (typeof reject === "function") {
            this._rejectionHandler0 =
                domain === null ? reject : domain.bind(reject);
        }
        if (typeof progress === "function") {
            this._progressHandler0 =
                domain === null ? progress : domain.bind(progress);
        }
    } else {
        var base = index * 5 - 5;
        this[base + 3] = promise;
        this[base + 4] = receiver;
        if (typeof fulfill === "function") {
            this[base + 0] =
                domain === null ? fulfill : domain.bind(fulfill);
        }
        if (typeof reject === "function") {
            this[base + 1] =
                domain === null ? reject : domain.bind(reject);
        }
        if (typeof progress === "function") {
            this[base + 2] =
                domain === null ? progress : domain.bind(progress);
        }
    }
    this._setLength(index + 1);
    return index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._attachExtraTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_attachExtraTrace (error, ignoreSelf)](#apidoc.element.rethinkdb._bluebird.prototype._attachExtraTrace)
- description and source-code
```javascript
_attachExtraTrace = function (error, ignoreSelf) {
    if (debugging && canAttachTrace(error)) {
        var trace = this._trace;
        if (trace !== undefined) {
            if (ignoreSelf) trace = trace._parent;
        }
        if (trace !== undefined) {
            trace.attachExtraTrace(error);
        } else if (!error.__stackCleaned__) {
            var parsed = CapturedTrace.parseStackAndMessage(error);
            util.notEnumerableProp(error, "stack",
                parsed.message + "\n" + parsed.stack.join("\n"));
            util.notEnumerableProp(error, "__stackCleaned__", true);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._boundValue"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_boundValue ()](#apidoc.element.rethinkdb._bluebird.prototype._boundValue)
- description and source-code
```javascript
_boundValue = function () {
    var ret = this._boundTo;
    if (ret !== undefined) {
        if (ret instanceof Promise) {
            if (ret.isFulfilled()) {
                return ret.value();
            } else {
                return undefined;
            }
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._cancel"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cancel (reason)](#apidoc.element.rethinkdb._bluebird.prototype._cancel)
- description and source-code
```javascript
_cancel = function (reason) {
    if (!this.isCancellable()) return this;
    var parent;
    var promiseToReject = this;
    while ((parent = promiseToReject._cancellationParent) !== undefined &&
        parent.isCancellable()) {
        promiseToReject = parent;
    }
    this._unsetCancellable();
    promiseToReject._target()._rejectCallback(reason, false, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._cancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._cancellable)
- description and source-code
```javascript
_cancellable = function () {
    return (this._bitField & 67108864) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._captureStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_captureStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._captureStackTrace)
- description and source-code
```javascript
_captureStackTrace = function () {
    if (debugging) {
        this._trace = new CapturedTrace(this._peekContext());
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._cleanValues"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_cleanValues ()](#apidoc.element.rethinkdb._bluebird.prototype._cleanValues)
- description and source-code
```javascript
_cleanValues = function () {
    if (this._cancellable()) {
        this._cancellationParent = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._clearCallbackDataAtIndex"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_clearCallbackDataAtIndex (index)](#apidoc.element.rethinkdb._bluebird.prototype._clearCallbackDataAtIndex)
- description and source-code
```javascript
_clearCallbackDataAtIndex = function (index) {
    if (index === 0) {
        if (!this._isCarryingStackTrace()) {
            this._fulfillmentHandler0 = undefined;
        }
        this._rejectionHandler0 =
        this._progressHandler0 =
        this._receiver0 =
        this._promise0 = undefined;
    } else {
        var base = index * 5 - 5;
        this[base + 3] =
        this[base + 4] =
        this[base + 0] =
        this[base + 1] =
        this[base + 2] = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._doProgressWith"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_doProgressWith (progression)](#apidoc.element.rethinkdb._bluebird.prototype._doProgressWith)
- description and source-code
```javascript
_doProgressWith = function (progression) {
    var progressValue = progression.value;
    var handler = progression.handler;
    var promise = progression.promise;
    var receiver = progression.receiver;

    var ret = tryCatch(handler).call(receiver, progressValue);
    if (ret === errorObj) {
        if (ret.e != null &&
            ret.e.name !== "StopProgressPropagation") {
            var trace = util.canAttachTrace(ret.e)
                ? ret.e : new Error(util.toString(ret.e));
            promise._attachExtraTrace(trace);
            promise._progress(ret.e);
        }
    } else if (ret instanceof Promise) {
        ret._then(promise._progress, null, null, promise, undefined);
    } else {
        promise._progress(ret);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._ensurePossibleRejectionHandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_ensurePossibleRejectionHandled ()](#apidoc.element.rethinkdb._bluebird.prototype._ensurePossibleRejectionHandled)
- description and source-code
```javascript
_ensurePossibleRejectionHandled = function () {
    if ((this._bitField & 16777216) !== 0) return;
    this._setRejectionIsUnhandled();
    async.invokeLater(this._notifyUnhandledRejection, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._followee"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_followee ()](#apidoc.element.rethinkdb._bluebird.prototype._followee)
- description and source-code
```javascript
_followee = function () {
    return this._rejectionHandler0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._fulfill"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfill (value)](#apidoc.element.rethinkdb._bluebird.prototype._fulfill)
- description and source-code
```javascript
_fulfill = function (value) {
    if (this._isFollowingOrFulfilledOrRejected()) return;
    this._fulfillUnchecked(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._fulfillUnchecked"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfillUnchecked (value)](#apidoc.element.rethinkdb._bluebird.prototype._fulfillUnchecked)
- description and source-code
```javascript
_fulfillUnchecked = function (value) {
    if (value === this) {
        var err = makeSelfResolutionError();
        this._attachExtraTrace(err);
        return this._rejectUnchecked(err, undefined);
    }
    this._setFulfilled();
    this._settledValue = value;
    this._cleanValues();

    if (this._length() > 0) {
        this._queueSettlePromises();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._fulfillmentHandlerAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_fulfillmentHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._fulfillmentHandlerAt)
- description and source-code
```javascript
_fulfillmentHandlerAt = function (index) {
    return index === 0
        ? this._fulfillmentHandler0
        : this[index * 5 - 5 + 0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._getCarriedStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_getCarriedStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._getCarriedStackTrace)
- description and source-code
```javascript
_getCarriedStackTrace = function () {
    return this._isCarryingStackTrace()
        ? this._fulfillmentHandler0
        : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._getDisposer"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_getDisposer ()](#apidoc.element.rethinkdb._bluebird.prototype._getDisposer)
- description and source-code
```javascript
_getDisposer = function () {
    return this._disposer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._ignoreRejections"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_ignoreRejections ()](#apidoc.element.rethinkdb._bluebird.prototype._ignoreRejections)
- description and source-code
```javascript
_ignoreRejections = function () {
    this._unsetRejectionIsUnhandled();
    this._bitField = this._bitField | 16777216;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isBound"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isBound ()](#apidoc.element.rethinkdb._bluebird.prototype._isBound)
- description and source-code
```javascript
_isBound = function () {
    return (this._bitField & 131072) === 131072;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isCarryingStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isCarryingStackTrace ()](#apidoc.element.rethinkdb._bluebird.prototype._isCarryingStackTrace)
- description and source-code
```javascript
_isCarryingStackTrace = function () {
    return (this._bitField & 1048576) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isDisposable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isDisposable ()](#apidoc.element.rethinkdb._bluebird.prototype._isDisposable)
- description and source-code
```javascript
_isDisposable = function () {
    return (this._bitField & 262144) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isFinal"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFinal ()](#apidoc.element.rethinkdb._bluebird.prototype._isFinal)
- description and source-code
```javascript
_isFinal = function () {
    return (this._bitField & 33554432) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isFollowing"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFollowing ()](#apidoc.element.rethinkdb._bluebird.prototype._isFollowing)
- description and source-code
```javascript
_isFollowing = function () {
    return (this._bitField & 536870912) === 536870912;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isFollowingOrFulfilledOrRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFollowingOrFulfilledOrRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._isFollowingOrFulfilledOrRejected)
- description and source-code
```javascript
_isFollowingOrFulfilledOrRejected = function () {
    return (this._bitField & 939524096) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype._isFulfilled)
- description and source-code
```javascript
_isFulfilled = function () {
    return (this._bitField & 268435456) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isMigrated"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._isMigrated)
- description and source-code
```javascript
_isMigrated = function () {
    return (this._bitField & 4194304) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isPending"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isPending ()](#apidoc.element.rethinkdb._bluebird.prototype._isPending)
- description and source-code
```javascript
_isPending = function () {
    return (this._bitField & 402653184) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._isRejected)
- description and source-code
```javascript
_isRejected = function () {
    return (this._bitField & 134217728) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isRejectionUnhandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isRejectionUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._isRejectionUnhandled)
- description and source-code
```javascript
_isRejectionUnhandled = function () {
    return (this._bitField & 2097152) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isResolved"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isResolved ()](#apidoc.element.rethinkdb._bluebird.prototype._isResolved)
- description and source-code
```javascript
_isResolved = function () {
    return (this._bitField & 402653184) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isSettlePromisesQueued"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._isSettlePromisesQueued)
- description and source-code
```javascript
_isSettlePromisesQueued = function () {
    return (this._bitField &
            -1073741824) === -1073741824;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._isUnhandledRejectionNotified"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_isUnhandledRejectionNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._isUnhandledRejectionNotified)
- description and source-code
```javascript
_isUnhandledRejectionNotified = function () {
    return (this._bitField & 524288) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._length"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_length ()](#apidoc.element.rethinkdb._bluebird.prototype._length)
- description and source-code
```javascript
_length = function () {
    return this._bitField & 131071;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._migrateCallbacks"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_migrateCallbacks (follower, index)](#apidoc.element.rethinkdb._bluebird.prototype._migrateCallbacks)
- description and source-code
```javascript
_migrateCallbacks = function (follower, index) {
    var fulfill = follower._fulfillmentHandlerAt(index);
    var reject = follower._rejectionHandlerAt(index);
    var progress = follower._progressHandlerAt(index);
    var promise = follower._promiseAt(index);
    var receiver = follower._receiverAt(index);
    if (promise instanceof Promise) promise._setIsMigrated();
    if (receiver === undefined) receiver = UNDEFINED_BINDING;
    this._addCallbacks(fulfill, reject, progress, promise, receiver, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejection"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_notifyUnhandledRejection ()](#apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejection)
- description and source-code
```javascript
_notifyUnhandledRejection = function () {
    if (this._isRejectionUnhandled()) {
        var reason = this._getCarriedStackTrace() || this._settledValue;
        this._setUnhandledRejectionIsNotified();
        CapturedTrace.fireRejectionEvent("unhandledRejection",
                                      possiblyUnhandledRejection, reason, this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejectionIsHandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_notifyUnhandledRejectionIsHandled ()](#apidoc.element.rethinkdb._bluebird.prototype._notifyUnhandledRejectionIsHandled)
- description and source-code
```javascript
_notifyUnhandledRejectionIsHandled = function () {
    CapturedTrace.fireRejectionEvent("rejectionHandled",
                                  unhandledRejectionHandled, undefined, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._passThroughHandler"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_passThroughHandler (handler, isFinally)](#apidoc.element.rethinkdb._bluebird.prototype._passThroughHandler)
- description and source-code
```javascript
_passThroughHandler = function (handler, isFinally) {
    if (typeof handler !== "function") return this.then();

    var promiseAndHandler = {
        promise: this,
        handler: handler
    };

    return this._then(
            isFinally ? finallyHandler : tapHandler,
            isFinally ? finallyHandler : undefined, undefined,
            promiseAndHandler, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._peekContext"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_peekContext ()](#apidoc.element.rethinkdb._bluebird.prototype._peekContext)
- description and source-code
```javascript
function peekContext() {
    var lastIndex = contextStack.length - 1;
    if (lastIndex >= 0) {
        return contextStack[lastIndex];
    }
    return undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._popContext"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_popContext ()](#apidoc.element.rethinkdb._bluebird.prototype._popContext)
- description and source-code
```javascript
_popContext = function () {
    if (!isDebugging()) return;
    if (this._trace !== undefined) {
        contextStack.pop();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._progress"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progress (progressValue)](#apidoc.element.rethinkdb._bluebird.prototype._progress)
- description and source-code
```javascript
_progress = function (progressValue) {
    if (this._isFollowingOrFulfilledOrRejected()) return;
    this._target()._progressUnchecked(progressValue);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._progressHandlerAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progressHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._progressHandlerAt)
- description and source-code
```javascript
_progressHandlerAt = function (index) {
    return index === 0
        ? this._progressHandler0
        : this[(index << 2) + index - 5 + 2];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._progressUnchecked"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_progressUnchecked (progressValue)](#apidoc.element.rethinkdb._bluebird.prototype._progressUnchecked)
- description and source-code
```javascript
_progressUnchecked = function (progressValue) {
    var len = this._length();
    var progress = this._progress;
    for (var i = 0; i < len; i++) {
        var handler = this._progressHandlerAt(i);
        var promise = this._promiseAt(i);
        if (!(promise instanceof Promise)) {
            var receiver = this._receiverAt(i);
            if (typeof handler === "function") {
                handler.call(receiver, progressValue, promise);
            } else if (receiver instanceof PromiseArray &&
                       !receiver._isResolved()) {
                receiver._promiseProgressed(progressValue, promise);
            }
            continue;
        }

        if (typeof handler === "function") {
            async.invoke(this._doProgressWith, this, {
                handler: handler,
                promise: promise,
                receiver: this._receiverAt(i),
                value: progressValue
            });
        } else {
            async.invoke(progress, promise, progressValue);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._promiseAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_promiseAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._promiseAt)
- description and source-code
```javascript
_promiseAt = function (index) {
    return index === 0
        ? this._promise0
        : this[index * 5 - 5 + 3];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._propagateFrom"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_propagateFrom (parent, flags)](#apidoc.element.rethinkdb._bluebird.prototype._propagateFrom)
- description and source-code
```javascript
_propagateFrom = function (parent, flags) {
    if ((flags & 1) > 0 && parent._cancellable()) {
        this._setCancellable();
        this._cancellationParent = parent;
    }
    if ((flags & 4) > 0 && parent._isBound()) {
        this._setBoundTo(parent._boundTo);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._proxyPromiseArray"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_proxyPromiseArray (promiseArray, index)](#apidoc.element.rethinkdb._bluebird.prototype._proxyPromiseArray)
- description and source-code
```javascript
_proxyPromiseArray = function (promiseArray, index) {
    this._setProxyHandlers(promiseArray, index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._pushContext"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_pushContext ()](#apidoc.element.rethinkdb._bluebird.prototype._pushContext)
- description and source-code
```javascript
_pushContext = function () {
    if (!isDebugging()) return;
    if (this._trace !== undefined) {
        contextStack.push(this._trace);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._queueSettlePromises"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_queueSettlePromises ()](#apidoc.element.rethinkdb._bluebird.prototype._queueSettlePromises)
- description and source-code
```javascript
_queueSettlePromises = function () {
    async.settlePromises(this);
    this._setSettlePromisesQueued();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._reason"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_reason ()](#apidoc.element.rethinkdb._bluebird.prototype._reason)
- description and source-code
```javascript
_reason = function () {
    this._unsetRejectionIsUnhandled();
    return this._settledValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._receiverAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_receiverAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._receiverAt)
- description and source-code
```javascript
_receiverAt = function (index) {
    var ret = index === 0
        ? this._receiver0
        : this[
            index * 5 - 5 + 4];
    if (ret === UNDEFINED_BINDING) {
        return undefined;
    } else if (ret === undefined && this._isBound()) {
        return this._boundValue();
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._reject"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_reject (reason, carriedStackTrace)](#apidoc.element.rethinkdb._bluebird.prototype._reject)
- description and source-code
```javascript
_reject = function (reason, carriedStackTrace) {
    if (this._isFollowingOrFulfilledOrRejected()) return;
    this._rejectUnchecked(reason, carriedStackTrace);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._rejectCallback"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectCallback (reason, synchronous, shouldNotMarkOriginatingFromRejection)](#apidoc.element.rethinkdb._bluebird.prototype._rejectCallback)
- description and source-code
```javascript
_rejectCallback = function (reason, synchronous, shouldNotMarkOriginatingFromRejection) {
    if (!shouldNotMarkOriginatingFromRejection) {
        util.markAsOriginatingFromRejection(reason);
    }
    var trace = util.ensureErrorObject(reason);
    var hasStack = trace === reason;
    this._attachExtraTrace(trace, synchronous ? hasStack : false);
    this._reject(reason, hasStack ? undefined : trace);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._rejectUnchecked"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectUnchecked (reason, trace)](#apidoc.element.rethinkdb._bluebird.prototype._rejectUnchecked)
- description and source-code
```javascript
_rejectUnchecked = function (reason, trace) {
    if (reason === this) {
        var err = makeSelfResolutionError();
        this._attachExtraTrace(err);
        return this._rejectUnchecked(err);
    }
    this._setRejected();
    this._settledValue = reason;
    this._cleanValues();

    if (this._isFinal()) {
        async.throwLater(function(e) {
            if ("stack" in e) {
                async.invokeFirst(
                    CapturedTrace.unhandledRejection, undefined, e);
            }
            throw e;
        }, trace === undefined ? reason : trace);
        return;
    }

    if (trace !== undefined && trace !== reason) {
        this._setCarriedStackTrace(trace);
    }

    if (this._length() > 0) {
        this._queueSettlePromises();
    } else {
        this._ensurePossibleRejectionHandled();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._rejectUncheckedCheckError"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectUncheckedCheckError (reason)](#apidoc.element.rethinkdb._bluebird.prototype._rejectUncheckedCheckError)
- description and source-code
```javascript
_rejectUncheckedCheckError = function (reason) {
    var trace = util.ensureErrorObject(reason);
    this._rejectUnchecked(reason, trace === reason ? undefined : trace);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._rejectionHandlerAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_rejectionHandlerAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._rejectionHandlerAt)
- description and source-code
```javascript
_rejectionHandlerAt = function (index) {
    return index === 0
        ? this._rejectionHandler0
        : this[index * 5 - 5 + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._resolveCallback"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveCallback (value, shouldBind)](#apidoc.element.rethinkdb._bluebird.prototype._resolveCallback)
- description and source-code
```javascript
_resolveCallback = function (value, shouldBind) {
    if (this._isFollowingOrFulfilledOrRejected()) return;
    if (value === this)
        return this._rejectCallback(makeSelfResolutionError(), false, true);
    var maybePromise = tryConvertToPromise(value, this);
    if (!(maybePromise instanceof Promise)) return this._fulfill(value);

    var propagationFlags = 1 | (shouldBind ? 4 : 0);
    this._propagateFrom(maybePromise, propagationFlags);
    var promise = maybePromise._target();
    if (promise._isPending()) {
        var len = this._length();
        for (var i = 0; i < len; ++i) {
            promise._migrateCallbacks(this, i);
        }
        this._setFollowing();
        this._setLength(0);
        this._setFollowee(promise);
    } else if (promise._isFulfilled()) {
        this._fulfillUnchecked(promise._value());
    } else {
        this._rejectUnchecked(promise._reason(),
            promise._getCarriedStackTrace());
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._resolveFromResolver"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveFromResolver (resolver)](#apidoc.element.rethinkdb._bluebird.prototype._resolveFromResolver)
- description and source-code
```javascript
_resolveFromResolver = function (resolver) {
    var promise = this;
    this._captureStackTrace();
    this._pushContext();
    var synchronous = true;
    var r = tryCatch(resolver)(function(value) {
        if (promise === null) return;
        promise._resolveCallback(value);
        promise = null;
    }, function (reason) {
        if (promise === null) return;
        promise._rejectCallback(reason, synchronous);
        promise = null;
    });
    synchronous = false;
    this._popContext();

    if (r !== undefined && r === errorObj && promise !== null) {
        promise._rejectCallback(r.e, true, true);
        promise = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._resolveFromSyncValue"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_resolveFromSyncValue (value)](#apidoc.element.rethinkdb._bluebird.prototype._resolveFromSyncValue)
- description and source-code
```javascript
_resolveFromSyncValue = function (value) {
    if (value === util.errorObj) {
        this._rejectCallback(value.e, false, true);
    } else {
        this._resolveCallback(value, true);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setBoundTo"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setBoundTo (obj)](#apidoc.element.rethinkdb._bluebird.prototype._setBoundTo)
- description and source-code
```javascript
_setBoundTo = function (obj) {
    if (obj !== undefined) {
        this._bitField = this._bitField | 131072;
        this._boundTo = obj;
    } else {
        this._bitField = this._bitField & (~131072);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setCancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._setCancellable)
- description and source-code
```javascript
_setCancellable = function () {
    this._bitField = this._bitField | 67108864;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setCarriedStackTrace"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setCarriedStackTrace (capturedTrace)](#apidoc.element.rethinkdb._bluebird.prototype._setCarriedStackTrace)
- description and source-code
```javascript
_setCarriedStackTrace = function (capturedTrace) {
    this._bitField = this._bitField | 1048576;
    this._fulfillmentHandler0 = capturedTrace;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setDisposable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setDisposable (disposer)](#apidoc.element.rethinkdb._bluebird.prototype._setDisposable)
- description and source-code
```javascript
_setDisposable = function (disposer) {
    this._bitField = this._bitField | 262144;
    this._disposer = disposer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setFollowee"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFollowee (promise)](#apidoc.element.rethinkdb._bluebird.prototype._setFollowee)
- description and source-code
```javascript
_setFollowee = function (promise) {
    this._rejectionHandler0 = promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setFollowing"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFollowing ()](#apidoc.element.rethinkdb._bluebird.prototype._setFollowing)
- description and source-code
```javascript
_setFollowing = function () {
    this._bitField = this._bitField | 536870912;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype._setFulfilled)
- description and source-code
```javascript
_setFulfilled = function () {
    this._bitField = this._bitField | 268435456;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setIsFinal"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setIsFinal ()](#apidoc.element.rethinkdb._bluebird.prototype._setIsFinal)
- description and source-code
```javascript
_setIsFinal = function () {
    this._bitField = this._bitField | 33554432;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setIsMigrated"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setIsMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._setIsMigrated)
- description and source-code
```javascript
_setIsMigrated = function () {
    this._bitField = this._bitField | 4194304;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setLength"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setLength (len)](#apidoc.element.rethinkdb._bluebird.prototype._setLength)
- description and source-code
```javascript
_setLength = function (len) {
    this._bitField = (this._bitField & -131072) |
        (len & 131071);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setProxyHandlers"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setProxyHandlers (receiver, promiseSlotValue)](#apidoc.element.rethinkdb._bluebird.prototype._setProxyHandlers)
- description and source-code
```javascript
_setProxyHandlers = function (receiver, promiseSlotValue) {
    var index = this._length();

    if (index >= 131071 - 5) {
        index = 0;
        this._setLength(0);
    }
    if (index === 0) {
        this._promise0 = promiseSlotValue;
        this._receiver0 = receiver;
    } else {
        var base = index * 5 - 5;
        this[base + 3] = promiseSlotValue;
        this[base + 4] = receiver;
    }
    this._setLength(index + 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setRejected ()](#apidoc.element.rethinkdb._bluebird.prototype._setRejected)
- description and source-code
```javascript
_setRejected = function () {
    this._bitField = this._bitField | 134217728;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setRejectionIsUnhandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setRejectionIsUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._setRejectionIsUnhandled)
- description and source-code
```javascript
_setRejectionIsUnhandled = function () {
    this._bitField = this._bitField | 2097152;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setSettlePromisesQueued"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._setSettlePromisesQueued)
- description and source-code
```javascript
_setSettlePromisesQueued = function () {
    this._bitField = this._bitField | -1073741824;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._setUnhandledRejectionIsNotified"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_setUnhandledRejectionIsNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._setUnhandledRejectionIsNotified)
- description and source-code
```javascript
_setUnhandledRejectionIsNotified = function () {
    this._bitField = this._bitField | 524288;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAt"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseAt (index)](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAt)
- description and source-code
```javascript
_settlePromiseAt = function (index) {
    var promise = this._promiseAt(index);
    var isPromise = promise instanceof Promise;

    if (isPromise && promise._isMigrated()) {
        promise._unsetIsMigrated();
        return async.invoke(this._settlePromiseAt, this, index);
    }
    var handler = this._isFulfilled()
        ? this._fulfillmentHandlerAt(index)
        : this._rejectionHandlerAt(index);

    var carriedStackTrace =
        this._isCarryingStackTrace() ? this._getCarriedStackTrace() : undefined;
    var value = this._settledValue;
    var receiver = this._receiverAt(index);
    this._clearCallbackDataAtIndex(index);

    if (typeof handler === "function") {
        if (!isPromise) {
            handler.call(receiver, value, promise);
        } else {
            this._settlePromiseFromHandler(handler, receiver, value, promise);
        }
    } else if (receiver instanceof PromiseArray) {
        if (!receiver._isResolved()) {
            if (this._isFulfilled()) {
                receiver._promiseFulfilled(value, promise);
            }
            else {
                receiver._promiseRejected(value, promise);
            }
        }
    } else if (isPromise) {
        if (this._isFulfilled()) {
            promise._fulfill(value);
        } else {
            promise._reject(value, carriedStackTrace);
        }
    }

    if (index >= 4 && (index & 31) === 4)
        async.invokeLater(this._setLength, this, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAtPostResolution"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseAtPostResolution (index)](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseAtPostResolution)
- description and source-code
```javascript
_settlePromiseAtPostResolution = function (index) {
    if (this._isRejectionUnhandled()) this._unsetRejectionIsUnhandled();
    this._settlePromiseAt(index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._settlePromiseFromHandler"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromiseFromHandler ( handler, receiver, value, promise )](#apidoc.element.rethinkdb._bluebird.prototype._settlePromiseFromHandler)
- description and source-code
```javascript
_settlePromiseFromHandler = function ( handler, receiver, value, promise ) {
    if (promise._isRejected()) return;
    promise._pushContext();
    var x;
    if (receiver === APPLY && !this._isRejected()) {
        x = tryCatch(handler).apply(this._boundValue(), value);
    } else {
        x = tryCatch(handler).call(receiver, value);
    }
    promise._popContext();

    if (x === errorObj || x === promise || x === NEXT_FILTER) {
        var err = x === promise ? makeSelfResolutionError() : x.e;
        promise._rejectCallback(err, false, true);
    } else {
        promise._resolveCallback(x);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._settlePromises"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_settlePromises ()](#apidoc.element.rethinkdb._bluebird.prototype._settlePromises)
- description and source-code
```javascript
_settlePromises = function () {
    this._unsetSettlePromisesQueued();
    var len = this._length();
    for (var i = 0; i < len; i++) {
        this._settlePromiseAt(i);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._target"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_target ()](#apidoc.element.rethinkdb._bluebird.prototype._target)
- description and source-code
```javascript
_target = function () {
    var ret = this;
    while (ret._isFollowing()) ret = ret._followee();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._then"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_then ( didFulfill, didReject, didProgress, receiver, internalData )](#apidoc.element.rethinkdb._bluebird.prototype._then)
- description and source-code
```javascript
_then = function ( didFulfill, didReject, didProgress, receiver, internalData ) {
    var haveInternalData = internalData !== undefined;
    var ret = haveInternalData ? internalData : new Promise(INTERNAL);

    if (!haveInternalData) {
        ret._propagateFrom(this, 4 | 1);
        ret._captureStackTrace();
    }

    var target = this._target();
    if (target !== this) {
        if (receiver === undefined) receiver = this._boundTo;
        if (!haveInternalData) ret._setIsMigrated();
    }

    var callbackIndex = target._addCallbacks(didFulfill,
                                             didReject,
                                             didProgress,
                                             ret,
                                             receiver,
                                             getDomain());

    if (target._isResolved() && !target._isSettlePromisesQueued()) {
        async.invoke(
            target._settlePromiseAtPostResolution, target, callbackIndex);
    }

    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetCancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetCancellable)
- description and source-code
```javascript
_unsetCancellable = function () {
    this._bitField = this._bitField & (~67108864);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetDisposable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetDisposable ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetDisposable)
- description and source-code
```javascript
_unsetDisposable = function () {
    this._bitField = this._bitField & (~262144);
    this._disposer = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetIsMigrated"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetIsMigrated ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetIsMigrated)
- description and source-code
```javascript
_unsetIsMigrated = function () {
    this._bitField = this._bitField & (~4194304);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetRejectionIsUnhandled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetRejectionIsUnhandled ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetRejectionIsUnhandled)
- description and source-code
```javascript
_unsetRejectionIsUnhandled = function () {
    this._bitField = this._bitField & (~2097152);
    if (this._isUnhandledRejectionNotified()) {
        this._unsetUnhandledRejectionIsNotified();
        this._notifyUnhandledRejectionIsHandled();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetSettlePromisesQueued"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetSettlePromisesQueued ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetSettlePromisesQueued)
- description and source-code
```javascript
_unsetSettlePromisesQueued = function () {
    this._bitField = this._bitField & (~-1073741824);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._unsetUnhandledRejectionIsNotified"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_unsetUnhandledRejectionIsNotified ()](#apidoc.element.rethinkdb._bluebird.prototype._unsetUnhandledRejectionIsNotified)
- description and source-code
```javascript
_unsetUnhandledRejectionIsNotified = function () {
    this._bitField = this._bitField & (~524288);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._value"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_value ()](#apidoc.element.rethinkdb._bluebird.prototype._value)
- description and source-code
```javascript
_value = function () {
    return this._settledValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype._warn"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>_warn (message)](#apidoc.element.rethinkdb._bluebird.prototype._warn)
- description and source-code
```javascript
_warn = function (message) {
    var warning = new Warning(message);
    var ctx = this._peekContext();
    if (ctx) {
        ctx.attachExtraTrace(warning);
    } else {
        var parsed = CapturedTrace.parseStackAndMessage(warning);
        warning.stack = parsed.message + "\n" + parsed.stack.join("\n");
    }
    CapturedTrace.formatAndLogError(warning, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.all"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>all ()](#apidoc.element.rethinkdb._bluebird.prototype.all)
- description and source-code
```javascript
all = function () {
    return new PromiseArray(this).promise();
}
```
- example usage
```shell
...
          return pending.splice(pending.indexOf(p), 1);
        });
        return pending.push(p);
      }).then(nextCb)["catch"](function(err) {
        if ((err != null ? err.message : void 0) !== 'No more rows in the cursor.') {
          throw err;
        }
        return Promise.all(pending);
      });
    }
  };
})(this);
resPromise = nextCb().then(function() {
  if (errCb != null) {
    return errCb(null);
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.any"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>any ()](#apidoc.element.rethinkdb._bluebird.prototype.any)
- description and source-code
```javascript
any = function () {
    return any(this);
}
```
- example usage
```shell
...
    throw new error.ReqlDriverError("Cursor is closed.");
  });
} else {
  return _this._next().then(function(data) {
    if (pending.length < options.concurrency) {
      return data;
    }
    return Promise.any(pending)["catch"](Promise.AggregateError, function(errs) {
      throw errs[0];
    })["return"](data);
  }).then(function(data) {
    var p;
    p = userCb(data).then(function() {
      return pending.splice(pending.indexOf(p), 1);
    });
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.asCallback"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>asCallback (nodeback, options)](#apidoc.element.rethinkdb._bluebird.prototype.asCallback)
- description and source-code
```javascript
asCallback = function (nodeback, options) {
    if (typeof nodeback == "function") {
        var adapter = successAdapter;
        if (options !== undefined && Object(options).spread) {
            adapter = spreadAdapter;
        }
        this._then(
            adapter,
            errorAdapter,
            undefined,
            this,
            nodeback
        );
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.bind"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>bind (thisArg)](#apidoc.element.rethinkdb._bluebird.prototype.bind)
- description and source-code
```javascript
bind = function (thisArg) {
    var maybePromise = tryConvertToPromise(thisArg);
    var ret = new Promise(INTERNAL);
    ret._propagateFrom(this, 1);
    var target = this._target();

    ret._setBoundTo(maybePromise);
    if (maybePromise instanceof Promise) {
        var context = {
            promiseRejectionQueued: false,
            promise: ret,
            target: target,
            bindingPromise: maybePromise
        };
        target._then(INTERNAL, targetRejected, ret._progress, ret, context);
        maybePromise._then(
            bindingResolved, bindingRejected, ret._progress, ret, context);
    } else {
        ret._resolveCallback(target);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.call"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>call (methodName)](#apidoc.element.rethinkdb._bluebird.prototype.call)
- description and source-code
```javascript
call = function (methodName) {
    var $_len = arguments.length;var args = new Array($_len - 1); for(var $_i = 1; $_i < $_len; ++$_i) {args[$_i - 1] = arguments
[$_i];}
    if (!false) {
        if (canEvaluate) {
            var maybeCaller = getMethodCaller(methodName);
            if (maybeCaller !== null) {
                return this._then(
                    maybeCaller, undefined, undefined, args, undefined);
            }
        }
    }
    args.push(methodName);
    return this._then(caller, undefined, undefined, args, undefined);
}
```
- example usage
```shell
...



// Generated by CoffeeScript 1.10.0
var ArrayResult, AtomFeed, Cursor, EventEmitter, Feed, IterableResult, OrderByLimitFeed, Promise, UnionedFeed, ar, aropt, error,
mkErr, protoResponseType, setImmediate, util, varar,
  bind = function(fn, me){ return function(){ return fn.apply(me, arguments); }; },
  slice = [].slice,
  extend = function(child, parent) { for (var key in parent) { if (hasProp.call(parent, key)) child[key] = parent[key]; } function
 ctor() { this.constructor = child; } ctor.prototype = parent.prototype; child.prototype = new ctor(); child.__super__ = parent.
prototype; return child; },
  hasProp = {}.hasOwnProperty;

error = require('./errors');

util = require('./util');

protoResponseType = require('./proto-def').Response.ResponseType;
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.cancel"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>cancel (reason)](#apidoc.element.rethinkdb._bluebird.prototype.cancel)
- description and source-code
```javascript
cancel = function (reason) {
    if (!this.isCancellable()) return this;
    if (reason === undefined) reason = new CancellationError();
    async.invokeLater(this._cancel, this, reason);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.cancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>cancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.cancellable)
- description and source-code
```javascript
cancellable = function () {
    if (this._cancellable()) return this;
    async.enableTrampoline();
    this._setCancellable();
    this._cancellationParent = undefined;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.catch"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>catch (fn)](#apidoc.element.rethinkdb._bluebird.prototype.catch)
- description and source-code
```javascript
catch = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (typeof item === "function") {
                catchInstances[j++] = item;
            } else {
                return Promise.reject(
                    new TypeError("Catch filter must inherit from Error or be a simple predicate function\u000a\u000a    See http
://goo.gl/o84o68\u000a"));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        var catchFilter = new CatchFilter(catchInstances, fn, this);
        return this._then(undefined, catchFilter.doFilter, undefined,
            catchFilter, undefined);
    }
    return this._then(undefined, fn, undefined, undefined, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.caught"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>caught (fn)](#apidoc.element.rethinkdb._bluebird.prototype.caught)
- description and source-code
```javascript
caught = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (typeof item === "function") {
                catchInstances[j++] = item;
            } else {
                return Promise.reject(
                    new TypeError("Catch filter must inherit from Error or be a simple predicate function\u000a\u000a    See http
://goo.gl/o84o68\u000a"));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        var catchFilter = new CatchFilter(catchInstances, fn, this);
        return this._then(undefined, catchFilter.doFilter, undefined,
            catchFilter, undefined);
    }
    return this._then(undefined, fn, undefined, undefined, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.delay"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>delay (ms)](#apidoc.element.rethinkdb._bluebird.prototype.delay)
- description and source-code
```javascript
delay = function (ms) {
    return delay(this, ms);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.disposer"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>disposer (fn)](#apidoc.element.rethinkdb._bluebird.prototype.disposer)
- description and source-code
```javascript
disposer = function (fn) {
    if (typeof fn === "function") {
        return new FunctionDisposer(fn, this, createContext());
    }
    throw new TypeError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.done"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>done (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.done)
- description and source-code
```javascript
done = function (didFulfill, didReject, didProgress) {
    var promise = this._then(didFulfill, didReject, didProgress,
        undefined, undefined);
    promise._setIsFinal();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.each"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>each (fn)](#apidoc.element.rethinkdb._bluebird.prototype.each)
- description and source-code
```javascript
each = function (fn) {
    return PromiseReduce(this, fn, null, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.error"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>error (fn)](#apidoc.element.rethinkdb._bluebird.prototype.error)
- description and source-code
```javascript
error = function (fn) {
    return this.caught(util.originatesFromRejection, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.filter"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>filter (fn, options)](#apidoc.element.rethinkdb._bluebird.prototype.filter)
- description and source-code
```javascript
filter = function (fn, options) {
    return PromiseMap(this, fn, options, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.finally"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>finally (handler)](#apidoc.element.rethinkdb._bluebird.prototype.finally)
- description and source-code
```javascript
finally = function (handler) {
    return this._passThroughHandler(handler, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.fork"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>fork (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.fork)
- description and source-code
```javascript
fork = function (didFulfill, didReject, didProgress) {
    var ret = this._then(didFulfill, didReject, didProgress,
                         undefined, undefined);

    ret._setCancellable();
    ret._cancellationParent = undefined;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.get"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>get (propertyName)](#apidoc.element.rethinkdb._bluebird.prototype.get)
- description and source-code
```javascript
get = function (propertyName) {
    var isIndex = (typeof propertyName === "number");
    var getter;
    if (!isIndex) {
        if (canEvaluate) {
            var maybeGetter = getGetter(propertyName);
            getter = maybeGetter !== null ? maybeGetter : namedGetter;
        } else {
            getter = namedGetter;
        }
    } else {
        getter = indexedGetter;
    }
    return this._then(getter, undefined, undefined, propertyName, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.isCancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isCancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.isCancellable)
- description and source-code
```javascript
isCancellable = function () {
    return !this.isResolved() &&
        this._cancellable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isFulfilled ()](#apidoc.element.rethinkdb._bluebird.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return this._target()._isFulfilled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.isPending"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isPending ()](#apidoc.element.rethinkdb._bluebird.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return this._target()._isPending();
}
```
- example usage
```shell
...
    };
  })(this);
  return Promise.fromNode(fn).nodeify(cb);
});

IterableResult.prototype.close = varar(0, 1, function(cb) {
  if (this._closeCbPromise != null) {
    if (this._closeCbPromise.isPending()) {
      this._closeCbPromise = this._closeCbPromise.nodeify(cb);
    } else {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
    }
  } else {
    if (this._endFlag) {
      this._closeCbPromise = Promise.resolve().nodeify(cb);
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isRejected ()](#apidoc.element.rethinkdb._bluebird.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return this._target()._isRejected();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.isResolved"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>isResolved ()](#apidoc.element.rethinkdb._bluebird.prototype.isResolved)
- description and source-code
```javascript
isResolved = function () {
    return this._target()._isResolved();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.lastly"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>lastly (handler)](#apidoc.element.rethinkdb._bluebird.prototype.lastly)
- description and source-code
```javascript
lastly = function (handler) {
    return this._passThroughHandler(handler, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.map"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>map (fn, options)](#apidoc.element.rethinkdb._bluebird.prototype.map)
- description and source-code
```javascript
map = function (fn, options) {
    if (typeof fn !== "function") return apiRejection("fn must be a function\u000a\u000a    See http://goo.gl/916lJJ\u000a");

    return map(this, fn, options, null).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.nodeify"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>nodeify (nodeback, options)](#apidoc.element.rethinkdb._bluebird.prototype.nodeify)
- description and source-code
```javascript
nodeify = function (nodeback, options) {
    if (typeof nodeback == "function") {
        var adapter = successAdapter;
        if (options !== undefined && Object(options).spread) {
            adapter = spreadAdapter;
        }
        this._then(
            adapter,
            errorAdapter,
            undefined,
            this,
            nodeback
        );
    }
    return this;
}
```
- example usage
```shell
...
  }
  fn = (function(_this) {
    return function(cb) {
      _this._cbQueue.push(cb);
      return _this._promptNext();
    };
  })(this);
  return Promise.fromNode(fn).nodeify(cb);
});

IterableResult.prototype.close = varar(0, 1, function(cb) {
  if (this._closeCbPromise != null) {
    if (this._closeCbPromise.isPending()) {
      this._closeCbPromise = this._closeCbPromise.nodeify(cb);
    } else {
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.progressed"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>progressed (handler)](#apidoc.element.rethinkdb._bluebird.prototype.progressed)
- description and source-code
```javascript
progressed = function (handler) {
    return this._then(undefined, undefined, handler, undefined, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.props"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>props ()](#apidoc.element.rethinkdb._bluebird.prototype.props)
- description and source-code
```javascript
props = function () {
    return props(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.race"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>race ()](#apidoc.element.rethinkdb._bluebird.prototype.race)
- description and source-code
```javascript
race = function () {
    return race(this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.reason"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reason ()](#apidoc.element.rethinkdb._bluebird.prototype.reason)
- description and source-code
```javascript
reason = function () {
    var target = this._target();
    if (!target.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/hPuiwB\u000a
");
    }
    target._unsetRejectionIsUnhandled();
    return target._settledValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.reduce"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reduce (fn, initialValue)](#apidoc.element.rethinkdb._bluebird.prototype.reduce)
- description and source-code
```javascript
reduce = function (fn, initialValue) {
    return reduce(this, fn, initialValue, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.reflect"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>reflect ()](#apidoc.element.rethinkdb._bluebird.prototype.reflect)
- description and source-code
```javascript
reflect = function () {
    return this._then(reflect, reflect, undefined, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.return"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>return (value)](#apidoc.element.rethinkdb._bluebird.prototype.return)
- description and source-code
```javascript
return = function (value) {
    if (value === undefined) return this.then(returnUndefined);

    if (isPrimitive(value)) {
        return this._then(
            wrapper(value, 2),
            undefined,
            undefined,
            undefined,
            undefined
       );
    } else if (value instanceof Promise) {
        value._ignoreRejections();
    }
    return this._then(returner, undefined, undefined, value, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.settle"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>settle ()](#apidoc.element.rethinkdb._bluebird.prototype.settle)
- description and source-code
```javascript
settle = function () {
    return new SettledPromiseArray(this).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.some"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>some (howMany)](#apidoc.element.rethinkdb._bluebird.prototype.some)
- description and source-code
```javascript
some = function (howMany) {
    return some(this, howMany);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.spread"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>spread (didFulfill, didReject)](#apidoc.element.rethinkdb._bluebird.prototype.spread)
- description and source-code
```javascript
spread = function (didFulfill, didReject) {
    return this.all()._then(didFulfill, didReject, undefined, APPLY, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.tap"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>tap (handler)](#apidoc.element.rethinkdb._bluebird.prototype.tap)
- description and source-code
```javascript
tap = function (handler) {
    return this._passThroughHandler(handler, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.then"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>then (didFulfill, didReject, didProgress)](#apidoc.element.rethinkdb._bluebird.prototype.then)
- description and source-code
```javascript
then = function (didFulfill, didReject, didProgress) {
    if (isDebugging() && arguments.length > 0 &&
        typeof didFulfill !== "function" &&
        typeof didReject !== "function") {
        var msg = ".then() only accepts functions but was passed: " +
                util.classString(didFulfill);
        if (arguments.length > 1) {
            msg += ", " + util.classString(didReject);
        }
        this._warn(msg);
    }
    return this._then(didFulfill, didReject, didProgress,
        undefined, undefined);
}
```
- example usage
```shell
...
        handler(new error.ReqlDriverError("A two-argument row handler for eachAsync may only return undefined."));
      } else if (handlerCalled) {
        handler(handlerArg);
      }
      return doneChecking = true;
    });
  }
  return ret.then(function(data) {
    if (data === void 0 || typeof data === Promise) {
      return data;
    }
    throw new error.ReqlDriverError("Row handler for eachAsync may only return a Promise or undefined.");
  });
};
nextCb = (function(_this) {
...
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.thenReturn"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>thenReturn (value)](#apidoc.element.rethinkdb._bluebird.prototype.thenReturn)
- description and source-code
```javascript
thenReturn = function (value) {
    if (value === undefined) return this.then(returnUndefined);

    if (isPrimitive(value)) {
        return this._then(
            wrapper(value, 2),
            undefined,
            undefined,
            undefined,
            undefined
       );
    } else if (value instanceof Promise) {
        value._ignoreRejections();
    }
    return this._then(returner, undefined, undefined, value, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.thenThrow"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>thenThrow (reason)](#apidoc.element.rethinkdb._bluebird.prototype.thenThrow)
- description and source-code
```javascript
thenThrow = function (reason) {
    if (reason === undefined) return this.then(throwUndefined);

    if (isPrimitive(reason)) {
        return this._then(
            wrapper(reason, 1),
            undefined,
            undefined,
            undefined,
            undefined
       );
    }
    return this._then(thrower, undefined, undefined, reason, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.throw"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>throw (reason)](#apidoc.element.rethinkdb._bluebird.prototype.throw)
- description and source-code
```javascript
throw = function (reason) {
    if (reason === undefined) return this.then(throwUndefined);

    if (isPrimitive(reason)) {
        return this._then(
            wrapper(reason, 1),
            undefined,
            undefined,
            undefined,
            undefined
       );
    }
    return this._then(thrower, undefined, undefined, reason, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.timeout"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>timeout (ms, message)](#apidoc.element.rethinkdb._bluebird.prototype.timeout)
- description and source-code
```javascript
timeout = function (ms, message) {
    ms = +ms;
    var ret = this.then().cancellable();
    ret._cancellationParent = this;
    var handle = setTimeout(function timeoutTimeout() {
        afterTimeout(ret, message);
    }, ms);
    return ret._then(successClear, failureClear, undefined, handle, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>toJSON ()](#apidoc.element.rethinkdb._bluebird.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    var ret = {
        isFulfilled: false,
        isRejected: false,
        fulfillmentValue: undefined,
        rejectionReason: undefined
    };
    if (this.isFulfilled()) {
        ret.fulfillmentValue = this.value();
        ret.isFulfilled = true;
    } else if (this.isRejected()) {
        ret.rejectionReason = this.reason();
        ret.isRejected = true;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.toString"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>toString ()](#apidoc.element.rethinkdb._bluebird.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return "[object Promise]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.uncancellable"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>uncancellable ()](#apidoc.element.rethinkdb._bluebird.prototype.uncancellable)
- description and source-code
```javascript
uncancellable = function () {
    var ret = this.then();
    ret._unsetCancellable();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb._bluebird.prototype.value"></a>[function <span class="apidocSignatureSpan">rethinkdb._bluebird.prototype.</span>value ()](#apidoc.element.rethinkdb._bluebird.prototype.value)
- description and source-code
```javascript
value = function () {
    var target = this._target();
    if (!target.isFulfilled()) {
        throw new TypeError("cannot get fulfillment value of a non-fulfilled promise\u000a\u000a    See http://goo.gl/hc1DLj\u000a
");
    }
    return target._settledValue;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.cursor"></a>[module rethinkdb.cursor](#apidoc.module.rethinkdb.cursor)

#### <a name="apidoc.element.rethinkdb.cursor.AtomFeed"></a>[function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>AtomFeed ()](#apidoc.element.rethinkdb.cursor.AtomFeed)
- description and source-code
```javascript
function AtomFeed() {
  this._type = protoResponseType.SUCCESS_PARTIAL;
  AtomFeed.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.cursor.Cursor"></a>[function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>Cursor ()](#apidoc.element.rethinkdb.cursor.Cursor)
- description and source-code
```javascript
function Cursor() {
  this._type = protoResponseType.SUCCESS_PARTIAL;
  Cursor.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.cursor.Feed"></a>[function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>Feed ()](#apidoc.element.rethinkdb.cursor.Feed)
- description and source-code
```javascript
function Feed() {
  this._type = protoResponseType.SUCCESS_PARTIAL;
  Feed.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.cursor.OrderByLimitFeed"></a>[function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>OrderByLimitFeed ()](#apidoc.element.rethinkdb.cursor.OrderByLimitFeed)
- description and source-code
```javascript
function OrderByLimitFeed() {
  this._type = protoResponseType.SUCCESS_PARTIAL;
  OrderByLimitFeed.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.cursor.makeIterable"></a>[function <span class="apidocSignatureSpan">rethinkdb.cursor.</span>makeIterable (response)](#apidoc.element.rethinkdb.cursor.makeIterable)
- description and source-code
```javascript
makeIterable = function (response) {
  var method, name, ref;
  response.__proto__ = {};
  ref = ArrayResult.prototype;
  for (name in ref) {
    method = ref[name];
    if (name !== 'constructor') {
      if (name === '_next') {
        response.__proto__['next'] = method;
        response.__proto__['_next'] = method;
      } else {
        response.__proto__[name] = method;
      }
    }
  }
  response.__proto__.__proto__ = [].__proto__;
  return response;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net"></a>[module rethinkdb.net](#apidoc.module.rethinkdb.net)

#### <a name="apidoc.element.rethinkdb.net.Connection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection)
- description and source-code
```javascript
function Connection(host, callback) {
  var conCallback, errCallback;
  if (typeof host === 'undefined') {
    host = {};
  } else if (typeof host === 'string') {
    host = {
      host: host
    };
  }
  this.host = host.host || this.DEFAULT_HOST;
  this.port = host.port || this.DEFAULT_PORT;
  this.db = host.db;
  this.authKey = host.authKey || this.DEFAULT_AUTH_KEY;
  this.timeout = host.timeout || this.DEFAULT_TIMEOUT;
  if (typeof host.ssl === 'boolean' && host.ssl) {
    this.ssl = {};
  } else if (typeof host.ssl === 'object') {
    this.ssl = host.ssl;
  } else {
    this.ssl = false;
  }
  this.outstandingCallbacks = {};
  this.nextToken = 1;
  this.open = false;
  this.closing = false;
  this.buffer = new Buffer(0);
  this._events = this._events || {};
  errCallback = (function(_this) {
    return function(e) {
      _this.removeListener('connect', conCallback);
      if (e instanceof err.ReqlError) {
        return callback(e);
      } else {
        return callback(new err.ReqlDriverError("Could not connect to " + _this.host + ":" + _this.port + ".\n" + e.message));
      }
    };
  })(this);
  this.once('error', errCallback);
  conCallback = (function(_this) {
    return function() {
      _this.removeListener('error', errCallback);
      _this.open = true;
      return callback(null, _this);
    };
  })(this);
  this.once('connect', conCallback);
  this._closePromise = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection)
- description and source-code
```javascript
function HttpConnection(host, callback) {
  var protocol, url, xhr;
  if (!HttpConnection.isAvailable()) {
    throw new err.ReqlDriverError("XMLHttpRequest is not available in this environment");
  }
  HttpConnection.__super__.constructor.call(this, host, callback);
  protocol = host.protocol === 'https' ? 'https' : this.DEFAULT_PROTOCOL;
  url = protocol + "://" + this.host + ":" + this.port + host.pathname + "ajax/reql/";
  xhr = new XMLHttpRequest;
  xhr.open("POST", url + ("open-new-connection?cacheBuster=" + (Math.random())), true);
  xhr.responseType = "text";
  xhr.onreadystatechange = (function(_this) {
    return function(e) {
      if (xhr.readyState === 4) {
        if (xhr.status === 200) {
          _this._url = url;
          _this._connId = xhr.response;
          return _this.emit('connect');
        } else {
          return _this.emit('error', new err.ReqlDriverError("XHR error, http status " + xhr.status + "."));
        }
      }
    };
  })(this);
  xhr.send();
  this.xhr = xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection)
- description and source-code
```javascript
function TcpConnection(host, callback) {
  var timeout;
  if (!TcpConnection.isAvailable()) {
    throw new err.ReqlDriverError("TCP sockets are not available in this environment");
  }
  TcpConnection.__super__.constructor.call(this, host, callback);
  if (this.ssl) {
    this.ssl.host = this.host;
    this.ssl.port = this.port;
    this.rawSocket = tls.connect(this.ssl);
  } else {
    this.rawSocket = net.connect(this.port, this.host);
  }
  this.rawSocket.setNoDelay();
  this.rawSocket.setKeepAlive(true);
  timeout = setTimeout(((function(_this) {
    return function() {
      _this.rawSocket.destroy();
      return _this.emit('error', new err.ReqlTimeoutError("Could not connect to " + _this.host + ":" + _this.port + ", operation
 timed out."));
    };
  })(this)), this.timeout * 1000);
  this.rawSocket.once('error', (function(_this) {
    return function() {
      return clearTimeout(timeout);
    };
  })(this));
  this.rawSocket.once('connect', (function(_this) {
    return function() {
      var auth_i, auth_r, auth_salt, client_first_message_bare, compare_digest, handshake_callback, handshake_error, max, message
, min, nullbyte, pbkdf2_hmac, protocol, r_string, server_first_message, server_signature, state, version, xor_bytes;
      version = new Buffer(4);
      version.writeUInt32LE(protoVersion, 0);
      protocol = new Buffer(4);
      protocol.writeUInt32LE(protoProtocol, 0);
      r_string = new Buffer(crypto.randomBytes(18)).toString('base64');
      _this.rawSocket.user = host["user"];
      _this.rawSocket.password = host["password"];
      if (_this.rawSocket.user === void 0) {
        _this.rawSocket.user = "admin";
      }
      if (_this.rawSocket.password === void 0) {
        _this.rawSocket.password = "";
      }
      client_first_message_bare = "n=" + _this.rawSocket.user + ",r=" + r_string;
      message = JSON.stringify({
        protocol_version: protoVersionNumber,
        authentication_method: "SCRAM-SHA-256",
        authentication: "n,," + client_first_message_bare
      });
      nullbyte = new Buffer('\0', "binary");
      _this.rawSocket.write(Buffer.concat([version, Buffer(message.toString()), nullbyte]));
      state = 1;
      min = 0;
      max = 0;
      server_first_message = "";
      server_signature = "";
      auth_r = "";
      auth_salt = "";
      auth_i = 0;
      xor_bytes = function(a, b) {
        var i, k, len, ref, res;
        res = [];
        len = Math.min(a.length, b.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          res.push(a[i] ^ b[i]);
        }
        return new Buffer(res);
      };
      pbkdf2_hmac = function(password, salt, iterations) {
        var c, cache_string, k, mac, ref, t, u;
        cache_string = password.toString("base64") + "," + salt.toString("base64") + "," + iterations.toString();
        if (pbkdf2_cache[cache_string]) {
          return pbkdf2_cache[cache_string];
        }
        mac = crypto.createHmac("sha256", password);
        mac.update(salt);
        mac.update("\x00\x00\x00\x01");
        u = mac.digest();
        t = u;
        for (c = k = 0, ref = iterations - 1; 0 <= ref ? k < ref : k > ref; c = 0 <= ref ? ++k : --k) {
          mac = crypto.createHmac("sha256", password);
          mac.update(t);
          t = mac.digest();
          u = xor_bytes(u, t);
        }
        pbkdf2_cache[cache_string] = u;
        return u;
      };
      compare_digest = function(a, b) {
        var i, k, left, len, ref, result, right;
        left = void 0;
        right = b;
        result = void 0;
        if (a.length === b.length) {
          left = a;
          result = 0;
        }
        if (a.length !== b.length) {
          left = b;
          result = 1;
        }
        len = Math.min(left.length, right.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          result |= left[i] ^ right[i];
        }
        return result === 0;
      };
      handshake_error = function(code, message) {
        if ((10 <= code & ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.connect"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>connect ()](#apidoc.element.rethinkdb.net.connect)
- description and source-code
```javascript
connect = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.isConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>isConnection (connection)](#apidoc.element.rethinkdb.net.isConnection)
- description and source-code
```javascript
isConnection = function (connection) {
  return connection instanceof Connection;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.Connection"></a>[module rethinkdb.net.Connection](#apidoc.module.rethinkdb.net.Connection)

#### <a name="apidoc.element.rethinkdb.net.Connection.Connection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>Connection (host, callback)](#apidoc.element.rethinkdb.net.Connection.Connection)
- description and source-code
```javascript
function Connection(host, callback) {
  var conCallback, errCallback;
  if (typeof host === 'undefined') {
    host = {};
  } else if (typeof host === 'string') {
    host = {
      host: host
    };
  }
  this.host = host.host || this.DEFAULT_HOST;
  this.port = host.port || this.DEFAULT_PORT;
  this.db = host.db;
  this.authKey = host.authKey || this.DEFAULT_AUTH_KEY;
  this.timeout = host.timeout || this.DEFAULT_TIMEOUT;
  if (typeof host.ssl === 'boolean' && host.ssl) {
    this.ssl = {};
  } else if (typeof host.ssl === 'object') {
    this.ssl = host.ssl;
  } else {
    this.ssl = false;
  }
  this.outstandingCallbacks = {};
  this.nextToken = 1;
  this.open = false;
  this.closing = false;
  this.buffer = new Buffer(0);
  this._events = this._events || {};
  errCallback = (function(_this) {
    return function(e) {
      _this.removeListener('connect', conCallback);
      if (e instanceof err.ReqlError) {
        return callback(e);
      } else {
        return callback(new err.ReqlDriverError("Could not connect to " + _this.host + ":" + _this.port + ".\n" + e.message));
      }
    };
  })(this);
  this.once('error', errCallback);
  conCallback = (function(_this) {
    return function() {
      _this.removeListener('error', errCallback);
      _this.open = true;
      return callback(null, _this);
    };
  })(this);
  this.once('connect', conCallback);
  this._closePromise = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.EventEmitter"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.Connection.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.init"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>init ()](#apidoc.element.rethinkdb.net.Connection.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.listenerCount"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.Connection.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.Connection.prototype"></a>[module rethinkdb.net.Connection.prototype](#apidoc.module.rethinkdb.net.Connection.prototype)

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._continueQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_continueQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._continueQuery)
- description and source-code
```javascript
_continueQuery = function (token) {
  var query;
  if (!this.open) {
    throw new err.ReqlDriverError("Connection is closed.");
  }
  query = {
    type: protoQueryType.CONTINUE,
    token: token
  };
  return this._sendQuery(query);
}
```
- example usage
```shell
...
  }
};

IterableResult.prototype._promptCont = function() {
  if ((!this._contFlag) && (!this._endFlag) && this._conn.isOpen()) {
    this._contFlag = true;
    this._outstandingRequests += 1;
    return this._conn._continueQuery(this._token);
  }
};

IterableResult.prototype.hasNext = function() {
  throw new error.ReqlDriverError("The 'hasNext' command has been removed since 1.13. Use 'next' instead.");
};
...
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._data"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_data (buf)](#apidoc.element.rethinkdb.net.Connection.prototype._data)
- description and source-code
```javascript
_data = function (buf) {
  var response, responseBuffer, responseLength, results, token;
  this.buffer = Buffer.concat([this.buffer, buf]);
  results = [];
  while (this.buffer.length >= 12) {
    token = this.buffer.readUInt32LE(0) + 0x100000000 * this.buffer.readUInt32LE(4);
    responseLength = this.buffer.readUInt32LE(8);
    if (!(this.buffer.length >= (12 + responseLength))) {
      break;
    }
    responseBuffer = this.buffer.slice(12, responseLength + 12);
    response = JSON.parse(responseBuffer);
    this._processResponse(response, token);
    results.push(this.buffer = this.buffer.slice(12 + responseLength));
  }
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._delQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_delQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._delQuery)
- description and source-code
```javascript
_delQuery = function (token) {
  return delete this.outstandingCallbacks[token];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._endQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_endQuery (token)](#apidoc.element.rethinkdb.net.Connection.prototype._endQuery)
- description and source-code
```javascript
_endQuery = function (token) {
  var query;
  if (!this.open) {
    throw new err.ReqlDriverError("Connection is closed.");
  }
  query = {
    type: protoQueryType.STOP,
    token: token
  };
  return this._sendQuery(query);
}
```
- example usage
```shell
...
              return reject(err);
            } else {
              return resolve();
            }
          };
          _this._closeAsap = true;
          _this._outstandingRequests += 1;
          return _this._conn._endQuery(_this._token);
        };
      })(this)).nodeify(cb);
    }
  }
  return this._closeCbPromise;
});
...
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._processResponse"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_processResponse (response, token)](#apidoc.element.rethinkdb.net.Connection.prototype._processResponse)
- description and source-code
```javascript
_processResponse = function (response, token) {
  var cb, cursor, errType, feed, k, len1, note, opts, profile, ref, ref1, root;
  profile = response.p;
  if (this.outstandingCallbacks[token] != null) {
    ref = this.outstandingCallbacks[token], cb = ref.cb, root = ref.root, cursor = ref.cursor, opts = ref.opts, feed = ref.feed;
    if (cursor != null) {
      cursor._addResponse(response);
      if (cursor._endFlag && cursor._outstandingRequests === 0) {
        return this._delQuery(token);
      }
    } else if (cb != null) {
      switch (response.t) {
        case protoResponseType.COMPILE_ERROR:
          cb(mkErr(err.ReqlServerCompileError, response, root));
          return this._delQuery(token);
        case protoResponseType.CLIENT_ERROR:
          cb(mkErr(err.ReqlDriverError, response, root));
          return this._delQuery(token);
        case protoResponseType.RUNTIME_ERROR:
          errType = util.errorClass(response.e);
          cb(mkErr(errType, response, root));
          return this._delQuery(token);
        case protoResponseType.SUCCESS_ATOM:
          response = mkAtom(response, opts);
          if (Array.isArray(response)) {
            response = cursors.makeIterable(response);
          }
          if (profile != null) {
            response = {
              profile: profile,
              value: response
            };
          }
          cb(null, response);
          return this._delQuery(token);
        case protoResponseType.SUCCESS_PARTIAL:
          cursor = null;
          ref1 = response.n;
          for (k = 0, len1 = ref1.length; k < len1; k++) {
            note = ref1[k];
            switch (note) {
              case protodef.Response.ResponseNote.SEQUENCE_FEED:
                if (cursor == null) {
                  cursor = new cursors.Feed(this, token, opts, root);
                }
                break;
              case protodef.Response.ResponseNote.UNIONED_FEED:
                if (cursor == null) {
                  cursor = new cursors.UnionedFeed(this, token, opts, root);
                }
                break;
              case protodef.Response.ResponseNote.ATOM_FEED:
                if (cursor == null) {
                  cursor = new cursors.AtomFeed(this, token, opts, root);
                }
                break;
              case protodef.Response.ResponseNote.ORDER_BY_LIMIT_FEED:
                if (cursor == null) {
                  cursor = new cursors.OrderByLimitFeed(this, token, opts, root);
                }
            }
          }
          if (cursor == null) {
            cursor = new cursors.Cursor(this, token, opts, root);
          }
          this.outstandingCallbacks[token].cursor = cursor;
          if (profile != null) {
            return cb(null, {
              profile: profile,
              value: cursor._addResponse(response)
            });
          } else {
            return cb(null, cursor._addResponse(response));
          }
          break;
        case protoResponseType.SUCCESS_SEQUENCE:
          cursor = new cursors.Cursor(this, token, opts, root);
          this._delQuery(token);
          if (profile != null) {
            return cb(null, {
              profile: profile,
              value: cursor._addResponse(response)
            });
          } else {
            return cb(null, cursor._addResponse(response));
          }
          break;
        case protoResponseType.WAIT_COMPLETE:
          this._delQuery(token);
          return cb(null, null);
        case protoResponseType.SERVER_INFO:
          this._delQuery(token);
          response = mkAtom(response, opts);
          return cb(null, response);
        default:
          return cb(new err.ReqlDriverError("Unknown response type"));
      }
    }
  } else {

  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._sendQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_sendQuery (query)](#apidoc.element.rethinkdb.net.Connection.prototype._sendQuery)
- description and source-code
```javascript
_sendQuery = function (query) {
  var data;
  data = [query.type];
  if (!(query.query === void 0)) {
    data.push(query.query);
    if ((query.global_optargs != null) && Object.keys(query.global_optargs).length > 0) {
      data.push(query.global_optargs);
    }
  }
  return this._writeQuery(query.token, JSON.stringify(data));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype._start"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>_start (term, cb, opts)](#apidoc.element.rethinkdb.net.Connection.prototype._start)
- description and source-code
```javascript
_start = function (term, cb, opts) {
  var key, query, token, value;
  if (!this.open) {
    throw new err.ReqlDriverError("Connection is closed.");
  }
  token = this.nextToken++;
  query = {};
  query.global_optargs = {};
  query.type = protoQueryType.START;
  query.query = term.build();
  query.token = token;
  for (key in opts) {
    if (!hasProp.call(opts, key)) continue;
    value = opts[key];
    query.global_optargs[util.fromCamelCase(key)] = r.expr(value).build();
  }
  if ((opts.db != null) || (this.db != null)) {
    query.global_optargs.db = r.db(opts.db || this.db).build();
  }
  if (opts.noreply != null) {
    query.global_optargs['noreply'] = r.expr(!!opts.noreply).build();
  }
  if (opts.profile != null) {
    query.global_optargs['profile'] = r.expr(!!opts.profile).build();
  }
  if ((opts.noreply == null) || !opts.noreply) {
    this.outstandingCallbacks[token] = {
      cb: cb,
      root: term,
      opts: opts
    };
  }
  this._sendQuery(query);
  if ((opts.noreply != null) && opts.noreply && typeof cb === 'function') {
    return cb(null);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.cancel"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.Connection.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (args.length !== fun.length) {
    throw new err.ReqlDriverCompileError("Expected " + fun.length + " argument" + (plural(fun.length)) + " but found " + args.length
 + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.Connection.prototype.close)
- description and source-code
```javascript
close = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
...
      }
    }
  }
  this._contFlag = false;
  if (this._closeAsap === false) {
    this._promptNext();
  } else {
    this.close(this._closeCb);
  }
  return this;
};

IterableResult.prototype._getCallback = function() {
  var cb, immediateCb;
  this._iterations += 1;
...
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.Connection.prototype.constructor)
- description and source-code
```javascript
function Connection(host, callback) {
  var conCallback, errCallback;
  if (typeof host === 'undefined') {
    host = {};
  } else if (typeof host === 'string') {
    host = {
      host: host
    };
  }
  this.host = host.host || this.DEFAULT_HOST;
  this.port = host.port || this.DEFAULT_PORT;
  this.db = host.db;
  this.authKey = host.authKey || this.DEFAULT_AUTH_KEY;
  this.timeout = host.timeout || this.DEFAULT_TIMEOUT;
  if (typeof host.ssl === 'boolean' && host.ssl) {
    this.ssl = {};
  } else if (typeof host.ssl === 'object') {
    this.ssl = host.ssl;
  } else {
    this.ssl = false;
  }
  this.outstandingCallbacks = {};
  this.nextToken = 1;
  this.open = false;
  this.closing = false;
  this.buffer = new Buffer(0);
  this._events = this._events || {};
  errCallback = (function(_this) {
    return function(e) {
      _this.removeListener('connect', conCallback);
      if (e instanceof err.ReqlError) {
        return callback(e);
      } else {
        return callback(new err.ReqlDriverError("Could not connect to " + _this.host + ":" + _this.port + ".\n" + e.message));
      }
    };
  })(this);
  this.once('error', errCallback);
  conCallback = (function(_this) {
    return function() {
      _this.removeListener('error', errCallback);
      _this.open = true;
      return callback(null, _this);
    };
  })(this);
  this.once('connect', conCallback);
  this._closePromise = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.isOpen"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>isOpen ()](#apidoc.element.rethinkdb.net.Connection.prototype.isOpen)
- description and source-code
```javascript
isOpen = function () {
  return this.open && !this.closing;
}
```
- example usage
```shell
...
          cb(new error.ReqlDriverError("Unknown response type for cursor"));
      }
    }
  }
};

IterableResult.prototype._promptCont = function() {
  if ((!this._contFlag) && (!this._endFlag) && this._conn.isOpen()) {
    this._contFlag = true;
    this._outstandingRequests += 1;
    return this._conn._continueQuery(this._token);
  }
};

IterableResult.prototype.hasNext = function() {
...
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.noreplyWait"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>noreplyWait ()](#apidoc.element.rethinkdb.net.Connection.prototype.noreplyWait)
- description and source-code
```javascript
noreplyWait = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.reconnect"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>reconnect ()](#apidoc.element.rethinkdb.net.Connection.prototype.reconnect)
- description and source-code
```javascript
reconnect = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.server"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>server ()](#apidoc.element.rethinkdb.net.Connection.prototype.server)
- description and source-code
```javascript
server = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.Connection.prototype.use"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.Connection.prototype.</span>use ()](#apidoc.element.rethinkdb.net.Connection.prototype.use)
- description and source-code
```javascript
use = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (args.length !== fun.length) {
    throw new err.ReqlDriverCompileError("Expected " + fun.length + " argument" + (plural(fun.length)) + " but found " + args.length
 + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.HttpConnection"></a>[module rethinkdb.net.HttpConnection](#apidoc.module.rethinkdb.net.HttpConnection)

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.HttpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>HttpConnection (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection.HttpConnection)
- description and source-code
```javascript
function HttpConnection(host, callback) {
  var protocol, url, xhr;
  if (!HttpConnection.isAvailable()) {
    throw new err.ReqlDriverError("XMLHttpRequest is not available in this environment");
  }
  HttpConnection.__super__.constructor.call(this, host, callback);
  protocol = host.protocol === 'https' ? 'https' : this.DEFAULT_PROTOCOL;
  url = protocol + "://" + this.host + ":" + this.port + host.pathname + "ajax/reql/";
  xhr = new XMLHttpRequest;
  xhr.open("POST", url + ("open-new-connection?cacheBuster=" + (Math.random())), true);
  xhr.responseType = "text";
  xhr.onreadystatechange = (function(_this) {
    return function(e) {
      if (xhr.readyState === 4) {
        if (xhr.status === 200) {
          _this._url = url;
          _this._connId = xhr.response;
          return _this.emit('connect');
        } else {
          return _this.emit('error', new err.ReqlDriverError("XHR error, http status " + xhr.status + "."));
        }
      }
    };
  })(this);
  xhr.send();
  this.xhr = xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.EventEmitter"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.HttpConnection.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.init"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>init ()](#apidoc.element.rethinkdb.net.HttpConnection.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.isAvailable"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>isAvailable ()](#apidoc.element.rethinkdb.net.HttpConnection.isAvailable)
- description and source-code
```javascript
isAvailable = function () {
  return typeof XMLHttpRequest !== "undefined";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.listenerCount"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.HttpConnection.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.HttpConnection.prototype"></a>[module rethinkdb.net.HttpConnection.prototype](#apidoc.module.rethinkdb.net.HttpConnection.prototype)

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.prototype._writeQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>_writeQuery (token, data)](#apidoc.element.rethinkdb.net.HttpConnection.prototype._writeQuery)
- description and source-code
```javascript
_writeQuery = function (token, data) {
  var buf;
  buf = new Buffer(encodeURI(data).split(/%..|./).length - 1 + 8);
  buf.writeUInt32LE(token & 0xFFFFFFFF, 0);
  buf.writeUInt32LE(Math.floor(token / 0xFFFFFFFF), 4);
  buf.write(data, 8);
  return this.write(buf, token);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.prototype.cancel"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.HttpConnection.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  var xhr;
  if (this._connId != null) {
    this.xhr.abort();
    xhr = new XMLHttpRequest;
    xhr.open("POST", this._url + "close-connection?conn_id=" + this._connId, true);
    xhr.responseType = "arraybuffer";
    xhr.send();
    this._url = null;
    this._connId = null;
    return HttpConnection.__super__.cancel.call(this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.HttpConnection.prototype.close)
- description and source-code
```javascript
close = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
...
      }
    }
  }
  this._contFlag = false;
  if (this._closeAsap === false) {
    this._promptNext();
  } else {
    this.close(this._closeCb);
  }
  return this;
};

IterableResult.prototype._getCallback = function() {
  var cb, immediateCb;
  this._iterations += 1;
...
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.HttpConnection.prototype.constructor)
- description and source-code
```javascript
function HttpConnection(host, callback) {
  var protocol, url, xhr;
  if (!HttpConnection.isAvailable()) {
    throw new err.ReqlDriverError("XMLHttpRequest is not available in this environment");
  }
  HttpConnection.__super__.constructor.call(this, host, callback);
  protocol = host.protocol === 'https' ? 'https' : this.DEFAULT_PROTOCOL;
  url = protocol + "://" + this.host + ":" + this.port + host.pathname + "ajax/reql/";
  xhr = new XMLHttpRequest;
  xhr.open("POST", url + ("open-new-connection?cacheBuster=" + (Math.random())), true);
  xhr.responseType = "text";
  xhr.onreadystatechange = (function(_this) {
    return function(e) {
      if (xhr.readyState === 4) {
        if (xhr.status === 200) {
          _this._url = url;
          _this._connId = xhr.response;
          return _this.emit('connect');
        } else {
          return _this.emit('error', new err.ReqlDriverError("XHR error, http status " + xhr.status + "."));
        }
      }
    };
  })(this);
  xhr.send();
  this.xhr = xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.HttpConnection.prototype.write"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.HttpConnection.prototype.</span>write (chunk, token)](#apidoc.element.rethinkdb.net.HttpConnection.prototype.write)
- description and source-code
```javascript
write = function (chunk, token) {
  var i, view, xhr;
  xhr = new XMLHttpRequest;
  xhr.open("POST", this._url + "?conn_id=" + this._connId, true);
  xhr.responseType = "arraybuffer";
  xhr.onreadystatechange = (function(_this) {
    return function(e) {
      var b, buf;
      if (xhr.readyState === 4 && xhr.status === 200) {
        buf = new Buffer((function() {
          var k, len1, ref, results;
          ref = new Uint8Array(xhr.response);
          results = [];
          for (k = 0, len1 = ref.length; k < len1; k++) {
            b = ref[k];
            results.push(b);
          }
          return results;
        })());
        return _this._data(buf);
      }
    };
  })(this);
  xhr.onerror = (function(_this) {
    return function(e) {
      return _this.outstandingCallbacks[token].cb(new Error("This HTTP connection is not open"));
    };
  })(this);
  view = new Uint8Array(chunk.length);
  i = 0;
  while (i < chunk.length) {
    view[i] = chunk[i];
    i++;
  }
  xhr.send(view);
  return this.xhr = xhr;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.TcpConnection"></a>[module rethinkdb.net.TcpConnection](#apidoc.module.rethinkdb.net.TcpConnection)

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.TcpConnection"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.</span>TcpConnection (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection.TcpConnection)
- description and source-code
```javascript
function TcpConnection(host, callback) {
  var timeout;
  if (!TcpConnection.isAvailable()) {
    throw new err.ReqlDriverError("TCP sockets are not available in this environment");
  }
  TcpConnection.__super__.constructor.call(this, host, callback);
  if (this.ssl) {
    this.ssl.host = this.host;
    this.ssl.port = this.port;
    this.rawSocket = tls.connect(this.ssl);
  } else {
    this.rawSocket = net.connect(this.port, this.host);
  }
  this.rawSocket.setNoDelay();
  this.rawSocket.setKeepAlive(true);
  timeout = setTimeout(((function(_this) {
    return function() {
      _this.rawSocket.destroy();
      return _this.emit('error', new err.ReqlTimeoutError("Could not connect to " + _this.host + ":" + _this.port + ", operation
 timed out."));
    };
  })(this)), this.timeout * 1000);
  this.rawSocket.once('error', (function(_this) {
    return function() {
      return clearTimeout(timeout);
    };
  })(this));
  this.rawSocket.once('connect', (function(_this) {
    return function() {
      var auth_i, auth_r, auth_salt, client_first_message_bare, compare_digest, handshake_callback, handshake_error, max, message
, min, nullbyte, pbkdf2_hmac, protocol, r_string, server_first_message, server_signature, state, version, xor_bytes;
      version = new Buffer(4);
      version.writeUInt32LE(protoVersion, 0);
      protocol = new Buffer(4);
      protocol.writeUInt32LE(protoProtocol, 0);
      r_string = new Buffer(crypto.randomBytes(18)).toString('base64');
      _this.rawSocket.user = host["user"];
      _this.rawSocket.password = host["password"];
      if (_this.rawSocket.user === void 0) {
        _this.rawSocket.user = "admin";
      }
      if (_this.rawSocket.password === void 0) {
        _this.rawSocket.password = "";
      }
      client_first_message_bare = "n=" + _this.rawSocket.user + ",r=" + r_string;
      message = JSON.stringify({
        protocol_version: protoVersionNumber,
        authentication_method: "SCRAM-SHA-256",
        authentication: "n,," + client_first_message_bare
      });
      nullbyte = new Buffer('\0', "binary");
      _this.rawSocket.write(Buffer.concat([version, Buffer(message.toString()), nullbyte]));
      state = 1;
      min = 0;
      max = 0;
      server_first_message = "";
      server_signature = "";
      auth_r = "";
      auth_salt = "";
      auth_i = 0;
      xor_bytes = function(a, b) {
        var i, k, len, ref, res;
        res = [];
        len = Math.min(a.length, b.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          res.push(a[i] ^ b[i]);
        }
        return new Buffer(res);
      };
      pbkdf2_hmac = function(password, salt, iterations) {
        var c, cache_string, k, mac, ref, t, u;
        cache_string = password.toString("base64") + "," + salt.toString("base64") + "," + iterations.toString();
        if (pbkdf2_cache[cache_string]) {
          return pbkdf2_cache[cache_string];
        }
        mac = crypto.createHmac("sha256", password);
        mac.update(salt);
        mac.update("\x00\x00\x00\x01");
        u = mac.digest();
        t = u;
        for (c = k = 0, ref = iterations - 1; 0 <= ref ? k < ref : k > ref; c = 0 <= ref ? ++k : --k) {
          mac = crypto.createHmac("sha256", password);
          mac.update(t);
          t = mac.digest();
          u = xor_bytes(u, t);
        }
        pbkdf2_cache[cache_string] = u;
        return u;
      };
      compare_digest = function(a, b) {
        var i, k, left, len, ref, result, right;
        left = void 0;
        right = b;
        result = void 0;
        if (a.length === b.length) {
          left = a;
          result = 0;
        }
        if (a.length !== b.length) {
          left = b;
          result = 1;
        }
        len = Math.min(left.length, right.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          result |= left[i] ^ right[i];
        }
        return result === 0;
      };
      handshake_error = function(code, message) {
        if ((10 <= code & ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.EventEmitter"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>EventEmitter ()](#apidoc.element.rethinkdb.net.TcpConnection.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.init"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>init ()](#apidoc.element.rethinkdb.net.TcpConnection.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.isAvailable"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>isAvailable ()](#apidoc.element.rethinkdb.net.TcpConnection.isAvailable)
- description and source-code
```javascript
isAvailable = function () {
  return !process.browser;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.listenerCount"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.</span>listenerCount (emitter, type)](#apidoc.element.rethinkdb.net.TcpConnection.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.net.TcpConnection.prototype"></a>[module rethinkdb.net.TcpConnection.prototype](#apidoc.module.rethinkdb.net.TcpConnection.prototype)

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype._writeQuery"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>_writeQuery (token, data)](#apidoc.element.rethinkdb.net.TcpConnection.prototype._writeQuery)
- description and source-code
```javascript
_writeQuery = function (token, data) {
  var tokenBuf;
  tokenBuf = new Buffer(8);
  tokenBuf.writeUInt32LE(token & 0xFFFFFFFF, 0);
  tokenBuf.writeUInt32LE(Math.floor(token / 0xFFFFFFFF), 4);
  this.rawSocket.write(tokenBuf);
  return this.write(new Buffer(data));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.cancel"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>cancel ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  this.rawSocket.destroy();
  return TcpConnection.__super__.cancel.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.clientAddress"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>clientAddress ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.clientAddress)
- description and source-code
```javascript
clientAddress = function () {
  return this.rawSocket.localAddress;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.clientPort"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>clientPort ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.clientPort)
- description and source-code
```javascript
clientPort = function () {
  return this.rawSocket.localPort;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>close ()](#apidoc.element.rethinkdb.net.TcpConnection.prototype.close)
- description and source-code
```javascript
close = function () {
  var args;
  args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
  if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
    if ((min != null) && (max == null)) {
      throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
    }
    if ((max != null) && (min == null)) {
      throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
    }
    throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
  }
  return fun.apply(this, args);
}
```
- example usage
```shell
...
      }
    }
  }
  this._contFlag = false;
  if (this._closeAsap === false) {
    this._promptNext();
  } else {
    this.close(this._closeCb);
  }
  return this;
};

IterableResult.prototype._getCallback = function() {
  var cb, immediateCb;
  this._iterations += 1;
...
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>constructor (host, callback)](#apidoc.element.rethinkdb.net.TcpConnection.prototype.constructor)
- description and source-code
```javascript
function TcpConnection(host, callback) {
  var timeout;
  if (!TcpConnection.isAvailable()) {
    throw new err.ReqlDriverError("TCP sockets are not available in this environment");
  }
  TcpConnection.__super__.constructor.call(this, host, callback);
  if (this.ssl) {
    this.ssl.host = this.host;
    this.ssl.port = this.port;
    this.rawSocket = tls.connect(this.ssl);
  } else {
    this.rawSocket = net.connect(this.port, this.host);
  }
  this.rawSocket.setNoDelay();
  this.rawSocket.setKeepAlive(true);
  timeout = setTimeout(((function(_this) {
    return function() {
      _this.rawSocket.destroy();
      return _this.emit('error', new err.ReqlTimeoutError("Could not connect to " + _this.host + ":" + _this.port + ", operation
 timed out."));
    };
  })(this)), this.timeout * 1000);
  this.rawSocket.once('error', (function(_this) {
    return function() {
      return clearTimeout(timeout);
    };
  })(this));
  this.rawSocket.once('connect', (function(_this) {
    return function() {
      var auth_i, auth_r, auth_salt, client_first_message_bare, compare_digest, handshake_callback, handshake_error, max, message
, min, nullbyte, pbkdf2_hmac, protocol, r_string, server_first_message, server_signature, state, version, xor_bytes;
      version = new Buffer(4);
      version.writeUInt32LE(protoVersion, 0);
      protocol = new Buffer(4);
      protocol.writeUInt32LE(protoProtocol, 0);
      r_string = new Buffer(crypto.randomBytes(18)).toString('base64');
      _this.rawSocket.user = host["user"];
      _this.rawSocket.password = host["password"];
      if (_this.rawSocket.user === void 0) {
        _this.rawSocket.user = "admin";
      }
      if (_this.rawSocket.password === void 0) {
        _this.rawSocket.password = "";
      }
      client_first_message_bare = "n=" + _this.rawSocket.user + ",r=" + r_string;
      message = JSON.stringify({
        protocol_version: protoVersionNumber,
        authentication_method: "SCRAM-SHA-256",
        authentication: "n,," + client_first_message_bare
      });
      nullbyte = new Buffer('\0', "binary");
      _this.rawSocket.write(Buffer.concat([version, Buffer(message.toString()), nullbyte]));
      state = 1;
      min = 0;
      max = 0;
      server_first_message = "";
      server_signature = "";
      auth_r = "";
      auth_salt = "";
      auth_i = 0;
      xor_bytes = function(a, b) {
        var i, k, len, ref, res;
        res = [];
        len = Math.min(a.length, b.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          res.push(a[i] ^ b[i]);
        }
        return new Buffer(res);
      };
      pbkdf2_hmac = function(password, salt, iterations) {
        var c, cache_string, k, mac, ref, t, u;
        cache_string = password.toString("base64") + "," + salt.toString("base64") + "," + iterations.toString();
        if (pbkdf2_cache[cache_string]) {
          return pbkdf2_cache[cache_string];
        }
        mac = crypto.createHmac("sha256", password);
        mac.update(salt);
        mac.update("\x00\x00\x00\x01");
        u = mac.digest();
        t = u;
        for (c = k = 0, ref = iterations - 1; 0 <= ref ? k < ref : k > ref; c = 0 <= ref ? ++k : --k) {
          mac = crypto.createHmac("sha256", password);
          mac.update(t);
          t = mac.digest();
          u = xor_bytes(u, t);
        }
        pbkdf2_cache[cache_string] = u;
        return u;
      };
      compare_digest = function(a, b) {
        var i, k, left, len, ref, result, right;
        left = void 0;
        right = b;
        result = void 0;
        if (a.length === b.length) {
          left = a;
          result = 0;
        }
        if (a.length !== b.length) {
          left = b;
          result = 1;
        }
        len = Math.min(left.length, right.length);
        for (i = k = 0, ref = len; 0 <= ref ? k < ref : k > ref; i = 0 <= ref ? ++k : --k) {
          result |= left[i] ^ right[i];
        }
        return result === 0;
      };
      handshake_error = function(code, message) {
        if ((10 <= code & ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.net.TcpConnection.prototype.write"></a>[function <span class="apidocSignatureSpan">rethinkdb.net.TcpConnection.prototype.</span>write (chunk)](#apidoc.element.rethinkdb.net.TcpConnection.prototype.write)
- description and source-code
```javascript
write = function (chunk) {
  var lengthBuffer;
  lengthBuffer = new Buffer(4);
  lengthBuffer.writeUInt32LE(chunk.length, 0);
  this.rawSocket.write(lengthBuffer);
  return this.rawSocket.write(chunk);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdb.util"></a>[module rethinkdb.util](#apidoc.module.rethinkdb.util)

#### <a name="apidoc.element.rethinkdb.util.ar"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>ar (fun)](#apidoc.element.rethinkdb.util.ar)
- description and source-code
```javascript
ar = function (fun) {
  return function() {
    var args;
    args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
    if (args.length !== fun.length) {
      throw new err.ReqlDriverCompileError("Expected " + fun.length + " argument" + (plural(fun.length)) + " but found " + args.
length + ".");
    }
    return fun.apply(this, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.aropt"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>aropt (fun)](#apidoc.element.rethinkdb.util.aropt)
- description and source-code
```javascript
aropt = function (fun) {
  return function() {
    var args, expectedPosArgs, numPosArgs, perhapsOptDict;
    args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
    expectedPosArgs = fun.length - 1;
    perhapsOptDict = args[expectedPosArgs];
    if ((perhapsOptDict != null) && (Object.prototype.toString.call(perhapsOptDict) !== '[object Object]')) {
      perhapsOptDict = null;
    }
    numPosArgs = args.length - (perhapsOptDict != null ? 1 : 0);
    if (expectedPosArgs !== numPosArgs) {
      if (expectedPosArgs !== 1) {
        throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " arguments (not including options) but found " + numPosArgs
 + ".");
      } else {
        throw new err.ReqlDriverCompileError("Expected " + expectedPosArgs + " argument (not including options) but found " + numPosArgs
 + ".");
      }
    }
    return fun.apply(this, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.errorClass"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>errorClass (errorType)](#apidoc.element.rethinkdb.util.errorClass)
- description and source-code
```javascript
errorClass = function (errorType) {
  switch (errorType) {
    case protoErrorType.QUERY_LOGIC:
      return err.ReqlQueryLogicError;
    case protoErrorType.NON_EXISTENCE:
      return err.ReqlNonExistenceError;
    case protoErrorType.RESOURCE_LIMIT:
      return err.ReqlResourceLimitError;
    case protoErrorType.USER:
      return err.ReqlUserError;
    case protoErrorType.INTERNAL:
      return err.ReqlInternalError;
    case protoErrorType.OP_FAILED:
      return err.ReqlOpFailedError;
    case protoErrorType.OP_INDETERMINATE:
      return err.ReqlOpIndeterminateError;
    case protoErrorType.PERMISSION_ERROR:
      return err.ReqlPermissionError;
    default:
      return err.ReqlRuntimeError;
  }
}
```
- example usage
```shell
...
      case protoResponseType.COMPILE_ERROR:
        this._closeCb(mkErr(error.ReqlServerCompileError, response, this._root));
        break;
      case protoResponseType.CLIENT_ERROR:
        this._closeCb(mkErr(error.ReqlClientError, response, this._root));
        break;
      case protoResponseType.RUNTIME_ERROR:
        this._closeCb(mkErr(util.errorClass(response.e), response, this._root));
        break;
      default:
        this._closeCb();
    }
  }
}
this._contFlag = false;
...
```

#### <a name="apidoc.element.rethinkdb.util.fromCamelCase"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>fromCamelCase (token)](#apidoc.element.rethinkdb.util.fromCamelCase)
- description and source-code
```javascript
fromCamelCase = function (token) {
  return token.replace(/[A-Z]/g, (function(_this) {
    return function(match) {
      return "_" + match.toLowerCase();
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.mkAtom"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkAtom (response, opts)](#apidoc.element.rethinkdb.util.mkAtom)
- description and source-code
```javascript
mkAtom = function (response, opts) {
  return recursivelyConvertPseudotype(response.r[0], opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.mkErr"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkErr (ErrClass, response, root)](#apidoc.element.rethinkdb.util.mkErr)
- description and source-code
```javascript
mkErr = function (ErrClass, response, root) {
  return new ErrClass(mkAtom(response), root, response.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.mkSeq"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>mkSeq (response, opts)](#apidoc.element.rethinkdb.util.mkSeq)
- description and source-code
```javascript
mkSeq = function (response, opts) {
  return recursivelyConvertPseudotype(response.r, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.recursivelyConvertPseudotype"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>recursivelyConvertPseudotype (obj, opts)](#apidoc.element.rethinkdb.util.recursivelyConvertPseudotype)
- description and source-code
```javascript
recursivelyConvertPseudotype = function (obj, opts) {
  var i, j, key, len, value;
  if (Array.isArray(obj)) {
    for (i = j = 0, len = obj.length; j < len; i = ++j) {
      value = obj[i];
      obj[i] = recursivelyConvertPseudotype(value, opts);
    }
  } else if (obj && typeof obj === 'object') {
    for (key in obj) {
      value = obj[key];
      obj[key] = recursivelyConvertPseudotype(value, opts);
    }
    obj = convertPseudotype(obj, opts);
  }
  return obj;
}
```
- example usage
```shell
...
    return cb;
  }
};

IterableResult.prototype._handleRow = function() {
  var cb, response, row;
  response = this._responses[0];
  row = util.recursivelyConvertPseudotype(response.r[this._responseIndex], this._opts);
  cb = this._getCallback();
  this._responseIndex += 1;
  if (this._responseIndex === response.r.length) {
    this._responses.shift();
    this._responseIndex = 0;
  }
  return cb(null, row);
...
```

#### <a name="apidoc.element.rethinkdb.util.toArrayBuffer"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>toArrayBuffer (node_buffer)](#apidoc.element.rethinkdb.util.toArrayBuffer)
- description and source-code
```javascript
toArrayBuffer = function (node_buffer) {
  var arr, i, j, len, value;
  arr = new Uint8Array(new ArrayBuffer(node_buffer.length));
  for (i = j = 0, len = node_buffer.length; j < len; i = ++j) {
    value = node_buffer[i];
    arr[i] = value;
  }
  return arr.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.toCamelCase"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>toCamelCase (token)](#apidoc.element.rethinkdb.util.toCamelCase)
- description and source-code
```javascript
toCamelCase = function (token) {
  return token.replace(/_[a-z]/g, (function(_this) {
    return function(match) {
      return match[1].toUpperCase();
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdb.util.varar"></a>[function <span class="apidocSignatureSpan">rethinkdb.util.</span>varar (min, max, fun)](#apidoc.element.rethinkdb.util.varar)
- description and source-code
```javascript
varar = function (min, max, fun) {
  return function() {
    var args;
    args = 1 <= arguments.length ? slice.call(arguments, 0) : [];
    if (((min != null) && args.length < min) || ((max != null) && args.length > max)) {
      if ((min != null) && (max == null)) {
        throw new err.ReqlDriverCompileError("Expected " + min + " or more arguments but found " + args.length + ".");
      }
      if ((max != null) && (min == null)) {
        throw new err.ReqlDriverCompileError("Expected " + max + " or fewer arguments but found " + args.length + ".");
      }
      throw new err.ReqlDriverCompileError("Expected between " + min + " and " + max + " arguments but found " + args.length + ".");
    }
    return fun.apply(this, args);
  };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
