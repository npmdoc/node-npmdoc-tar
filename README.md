# api documentation for  [tar (v2.2.1)](https://github.com/isaacs/node-tar#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-tar.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tar) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tar.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tar)
#### tar for node

[![NPM](https://nodei.co/npm/tar.png?downloads=true)](https://www.npmjs.com/package/tar)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tar/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-tar_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tar/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tar/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tar/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Isaac Z. Schlueter",
        "email": "i@izs.me",
        "url": "http://blog.izs.me/"
    },
    "bugs": {
        "url": "https://github.com/isaacs/node-tar/issues"
    },
    "dependencies": {
        "block-stream": "*",
        "fstream": "^1.0.2",
        "inherits": "2"
    },
    "description": "tar for node",
    "devDependencies": {
        "graceful-fs": "^4.1.2",
        "mkdirp": "^0.5.0",
        "rimraf": "1.x",
        "tap": "0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "8e4d2a256c0e2185c6b18ad694aec968b83cb1d1",
        "tarball": "https://registry.npmjs.org/tar/-/tar-2.2.1.tgz"
    },
    "gitHead": "52237e39d2eb68d22a32d9a98f1d762189fe6a3d",
    "homepage": "https://github.com/isaacs/node-tar#readme",
    "license": "ISC",
    "main": "tar.js",
    "maintainers": [
        {
            "name": "isaacs",
            "email": "isaacs@npmjs.com"
        },
        {
            "name": "othiym23",
            "email": "ogd@aoaioxxysz.net"
        },
        {
            "name": "soldair",
            "email": "soldair@gmail.com"
        },
        {
            "name": "zkat",
            "email": "kat@sykosomatic.org"
        }
    ],
    "name": "tar",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/isaacs/node-tar.git"
    },
    "scripts": {
        "test": "tap test/*.js"
    },
    "version": "2.2.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tar](#apidoc.module.tar)
1.  [function <span class="apidocSignatureSpan">tar.</span>Extract (opts)](#apidoc.element.tar.Extract)
1.  [function <span class="apidocSignatureSpan">tar.</span>Pack (props)](#apidoc.element.tar.Pack)
1.  [function <span class="apidocSignatureSpan">tar.</span>Parse ()](#apidoc.element.tar.Parse)
1.  [function <span class="apidocSignatureSpan">tar.</span>Parse.super_ (props, currentStat)](#apidoc.element.tar.Parse.super_)
1.  [function <span class="apidocSignatureSpan">tar.</span>buffer_entry ()](#apidoc.element.tar.buffer_entry)
1.  [function <span class="apidocSignatureSpan">tar.</span>entry (header, extended, global)](#apidoc.element.tar.entry)
1.  [function <span class="apidocSignatureSpan">tar.</span>entry_writer (props)](#apidoc.element.tar.entry_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>extended_header ()](#apidoc.element.tar.extended_header)
1.  [function <span class="apidocSignatureSpan">tar.</span>extended_header_writer (props)](#apidoc.element.tar.extended_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>global_header_writer (props)](#apidoc.element.tar.global_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>header (block)](#apidoc.element.tar.header)
1.  number <span class="apidocSignatureSpan">tar.</span>blockSize
1.  number <span class="apidocSignatureSpan">tar.</span>headerSize
1.  object <span class="apidocSignatureSpan">tar.</span>Extract.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Pack.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.Dir.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.File.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.Link.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.Proxy.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>Parse.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>buffer_entry.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>entry.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>entry_writer.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>extended_header.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>extended_header_writer.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>fieldEnds
1.  object <span class="apidocSignatureSpan">tar.</span>fieldOffs
1.  object <span class="apidocSignatureSpan">tar.</span>fieldSize
1.  object <span class="apidocSignatureSpan">tar.</span>fields
1.  object <span class="apidocSignatureSpan">tar.</span>header.prototype
1.  object <span class="apidocSignatureSpan">tar.</span>knownExtended
1.  object <span class="apidocSignatureSpan">tar.</span>modes
1.  object <span class="apidocSignatureSpan">tar.</span>numeric
1.  object <span class="apidocSignatureSpan">tar.</span>types

#### [module tar.Extract](#apidoc.module.tar.Extract)
1.  [function <span class="apidocSignatureSpan">tar.</span>Extract (opts)](#apidoc.element.tar.Extract.Extract)
1.  [function <span class="apidocSignatureSpan">tar.Extract.</span>super_ ()](#apidoc.element.tar.Extract.super_)

#### [module tar.Extract.prototype](#apidoc.module.tar.Extract.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Extract.prototype.</span>_streamEnd ()](#apidoc.element.tar.Extract.prototype._streamEnd)

#### [module tar.Pack](#apidoc.module.tar.Pack)
1.  [function <span class="apidocSignatureSpan">tar.</span>Pack (props)](#apidoc.element.tar.Pack.Pack)
1.  [function <span class="apidocSignatureSpan">tar.Pack.</span>super_ ()](#apidoc.element.tar.Pack.super_)

#### [module tar.Pack.prototype](#apidoc.module.tar.Pack.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>_process ()](#apidoc.element.tar.Pack.prototype._process)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>add (stream)](#apidoc.element.tar.Pack.prototype.add)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>addGlobal (props)](#apidoc.element.tar.Pack.prototype.addGlobal)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>destroy ()](#apidoc.element.tar.Pack.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>end ()](#apidoc.element.tar.Pack.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>pause ()](#apidoc.element.tar.Pack.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>resume ()](#apidoc.element.tar.Pack.prototype.resume)
1.  [function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>write ()](#apidoc.element.tar.Pack.prototype.write)

#### [module tar.Parse](#apidoc.module.tar.Parse)
1.  [function <span class="apidocSignatureSpan">tar.</span>Parse ()](#apidoc.element.tar.Parse.Parse)
1.  [function <span class="apidocSignatureSpan">tar.Parse.</span>create ()](#apidoc.element.tar.Parse.create)
1.  [function <span class="apidocSignatureSpan">tar.Parse.</span>super_ (props, currentStat)](#apidoc.element.tar.Parse.super_)

#### [module tar.Parse.prototype](#apidoc.module.tar.Parse.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_process (c)](#apidoc.element.tar.Parse.prototype._process)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_read ()](#apidoc.element.tar.Parse.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_startEntry (c)](#apidoc.element.tar.Parse.prototype._startEntry)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_streamEnd ()](#apidoc.element.tar.Parse.prototype._streamEnd)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>end (c)](#apidoc.element.tar.Parse.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>write (c)](#apidoc.element.tar.Parse.prototype.write)

#### [module tar.Parse.super_](#apidoc.module.tar.Parse.super_)
1.  [function <span class="apidocSignatureSpan">tar.Parse.</span>super_ ()](#apidoc.element.tar.Parse.super_.super_)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Dir (props)](#apidoc.element.tar.Parse.super_.Dir)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.</span>File (props)](#apidoc.element.tar.Parse.super_.File)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Link (props)](#apidoc.element.tar.Parse.super_.Link)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Proxy (props)](#apidoc.element.tar.Parse.super_.Proxy)
1.  object <span class="apidocSignatureSpan">tar.Parse.super_.</span>hardLinks

#### [module tar.Parse.super_.Dir.prototype](#apidoc.module.tar.Parse.super_.Dir.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>_getEntries ()](#apidoc.element.tar.Parse.super_.Dir.prototype._getEntries)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.Dir.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>disown (entry)](#apidoc.element.tar.Parse.super_.Dir.prototype.disown)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>emitEntry (entry)](#apidoc.element.tar.Parse.super_.Dir.prototype.emitEntry)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>getChildProps ()](#apidoc.element.tar.Parse.super_.Dir.prototype.getChildProps)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.Dir.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.Dir.prototype.resume)

#### [module tar.Parse.super_.File.prototype](#apidoc.module.tar.Parse.super_.File.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>_getStream ()](#apidoc.element.tar.Parse.super_.File.prototype._getStream)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.File.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.File.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.File.prototype.resume)

#### [module tar.Parse.super_.Link.prototype](#apidoc.module.tar.Parse.super_.Link.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Link.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.Link.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Link.prototype.</span>_stat (currentStat)](#apidoc.element.tar.Parse.super_.Link.prototype._stat)

#### [module tar.Parse.super_.Proxy.prototype](#apidoc.module.tar.Parse.super_.Proxy.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>_addProxy (proxy)](#apidoc.element.tar.Parse.super_.Proxy.prototype._addProxy)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>_stat ()](#apidoc.element.tar.Parse.super_.Proxy.prototype._stat)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>pause ()](#apidoc.element.tar.Parse.super_.Proxy.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>resume ()](#apidoc.element.tar.Parse.super_.Proxy.prototype.resume)

#### [module tar.Parse.super_.prototype](#apidoc.module.tar.Parse.super_.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>_stat (currentStat)](#apidoc.element.tar.Parse.super_.prototype._stat)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>pipe (dest)](#apidoc.element.tar.Parse.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.prototype.resume)

#### [module tar.Parse.super_.super_.prototype](#apidoc.module.tar.Parse.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>abort ()](#apidoc.element.tar.Parse.super_.super_.prototype.abort)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>destroy ()](#apidoc.element.tar.Parse.super_.super_.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>error (msg, code, th)](#apidoc.element.tar.Parse.super_.super_.prototype.error)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>info (msg, code)](#apidoc.element.tar.Parse.super_.super_.prototype.info)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.tar.Parse.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>warn (msg, code)](#apidoc.element.tar.Parse.super_.super_.prototype.warn)

#### [module tar.buffer_entry](#apidoc.module.tar.buffer_entry)
1.  [function <span class="apidocSignatureSpan">tar.</span>buffer_entry ()](#apidoc.element.tar.buffer_entry.buffer_entry)
1.  [function <span class="apidocSignatureSpan">tar.buffer_entry.</span>super_ (header, extended, global)](#apidoc.element.tar.buffer_entry.super_)

#### [module tar.buffer_entry.prototype](#apidoc.module.tar.buffer_entry.prototype)
1.  [function <span class="apidocSignatureSpan">tar.buffer_entry.prototype.</span>write (c)](#apidoc.element.tar.buffer_entry.prototype.write)

#### [module tar.entry](#apidoc.module.tar.entry)
1.  [function <span class="apidocSignatureSpan">tar.</span>entry (header, extended, global)](#apidoc.element.tar.entry.entry)
1.  [function <span class="apidocSignatureSpan">tar.entry.</span>super_ ()](#apidoc.element.tar.entry.super_)

#### [module tar.entry.prototype](#apidoc.module.tar.entry.prototype)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>_read ()](#apidoc.element.tar.entry.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>_setProps ()](#apidoc.element.tar.entry.prototype._setProps)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>abort ()](#apidoc.element.tar.entry.prototype.abort)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>end (c)](#apidoc.element.tar.entry.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>pause ()](#apidoc.element.tar.entry.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>resume ()](#apidoc.element.tar.entry.prototype.resume)
1.  [function <span class="apidocSignatureSpan">tar.entry.prototype.</span>write (c)](#apidoc.element.tar.entry.prototype.write)

#### [module tar.entry_writer](#apidoc.module.tar.entry_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>entry_writer (props)](#apidoc.element.tar.entry_writer.entry_writer)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.</span>super_ ()](#apidoc.element.tar.entry_writer.super_)

#### [module tar.entry_writer.prototype](#apidoc.module.tar.entry_writer.prototype)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>_header ()](#apidoc.element.tar.entry_writer.prototype._header)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>_process ()](#apidoc.element.tar.entry_writer.prototype._process)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>add (entry)](#apidoc.element.tar.entry_writer.prototype.add)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>destroy ()](#apidoc.element.tar.entry_writer.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>end (c)](#apidoc.element.tar.entry_writer.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>pause ()](#apidoc.element.tar.entry_writer.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>resume ()](#apidoc.element.tar.entry_writer.prototype.resume)
1.  [function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>write (c)](#apidoc.element.tar.entry_writer.prototype.write)

#### [module tar.extended_header](#apidoc.module.tar.extended_header)
1.  [function <span class="apidocSignatureSpan">tar.</span>extended_header ()](#apidoc.element.tar.extended_header.extended_header)
1.  [function <span class="apidocSignatureSpan">tar.extended_header.</span>super_ (header, extended, global)](#apidoc.element.tar.extended_header.super_)
1.  object <span class="apidocSignatureSpan">tar.extended_header.</span>states

#### [module tar.extended_header.prototype](#apidoc.module.tar.extended_header.prototype)
1.  [function <span class="apidocSignatureSpan">tar.extended_header.prototype.</span>_parse (c)](#apidoc.element.tar.extended_header.prototype._parse)

#### [module tar.extended_header_writer](#apidoc.module.tar.extended_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>extended_header_writer (props)](#apidoc.element.tar.extended_header_writer.extended_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.extended_header_writer.</span>super_ (props)](#apidoc.element.tar.extended_header_writer.super_)

#### [module tar.extended_header_writer.prototype](#apidoc.module.tar.extended_header_writer.prototype)
1.  [function <span class="apidocSignatureSpan">tar.extended_header_writer.prototype.</span>_encodeFields ()](#apidoc.element.tar.extended_header_writer.prototype._encodeFields)
1.  [function <span class="apidocSignatureSpan">tar.extended_header_writer.prototype.</span>end ()](#apidoc.element.tar.extended_header_writer.prototype.end)

#### [module tar.global_header_writer](#apidoc.module.tar.global_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.</span>global_header_writer (props)](#apidoc.element.tar.global_header_writer.global_header_writer)
1.  [function <span class="apidocSignatureSpan">tar.global_header_writer.</span>super_ (props)](#apidoc.element.tar.global_header_writer.super_)

#### [module tar.header](#apidoc.module.tar.header)
1.  [function <span class="apidocSignatureSpan">tar.</span>header (block)](#apidoc.element.tar.header.header)
1.  [function <span class="apidocSignatureSpan">tar.header.</span>decode (block)](#apidoc.element.tar.header.decode)
1.  [function <span class="apidocSignatureSpan">tar.header.</span>encode (obj)](#apidoc.element.tar.header.encode)
1.  [function <span class="apidocSignatureSpan">tar.header.</span>parseNumeric (f)](#apidoc.element.tar.header.parseNumeric)

#### [module tar.header.prototype](#apidoc.module.tar.header.prototype)
1.  [function <span class="apidocSignatureSpan">tar.header.prototype.</span>calcSum (block)](#apidoc.element.tar.header.prototype.calcSum)
1.  [function <span class="apidocSignatureSpan">tar.header.prototype.</span>checkSum (block)](#apidoc.element.tar.header.prototype.checkSum)
1.  [function <span class="apidocSignatureSpan">tar.header.prototype.</span>decode (block)](#apidoc.element.tar.header.prototype.decode)
1.  [function <span class="apidocSignatureSpan">tar.header.prototype.</span>encode (obj)](#apidoc.element.tar.header.prototype.encode)



# <a name="apidoc.module.tar"></a>[module tar](#apidoc.module.tar)

#### <a name="apidoc.element.tar.Extract"></a>[function <span class="apidocSignatureSpan">tar.</span>Extract (opts)](#apidoc.element.tar.Extract)
- description and source-code
```javascript
function Extract(opts) {
  if (!(this instanceof Extract)) return new Extract(opts)
  tar.Parse.apply(this)

  if (typeof opts !== "object") {
    opts = { path: opts }
  }

  // better to drop in cwd? seems more standard.
  opts.path = opts.path || path.resolve("node-tar-extract")
  opts.type = "Directory"
  opts.Directory = true

  // similar to --strip or --strip-components
  opts.strip = +opts.strip
  if (!opts.strip || opts.strip <= 0) opts.strip = 0

  this._fst = fstream.Writer(opts)

  this.pause()
  var me = this

  // Hardlinks in tarballs are relative to the root
  // of the tarball.  So, they need to be resolved against
  // the target directory in order to be created properly.
  me.on("entry", function (entry) {
    // if there's a "strip" argument, then strip off that many
    // path components.
    if (opts.strip) {
      var p = entry.path.split("/").slice(opts.strip).join("/")
      entry.path = entry.props.path = p
      if (entry.linkpath) {
        var lp = entry.linkpath.split("/").slice(opts.strip).join("/")
        entry.linkpath = entry.props.linkpath = lp
      }
    }
    if (entry.type === "Link") {
      entry.linkpath = entry.props.linkpath =
        path.join(opts.path, path.join("/", entry.props.linkpath))
    }

    if (entry.type === "SymbolicLink") {
      var dn = path.dirname(entry.path) || ""
      var linkpath = entry.props.linkpath
      var target = path.resolve(opts.path, dn, linkpath)
      if (target.indexOf(opts.path) !== 0) {
        linkpath = path.join(opts.path, path.join("/", linkpath))
      }
      entry.linkpath = entry.props.linkpath = linkpath
    }
  })

  this._fst.on("ready", function () {
    me.pipe(me._fst, { end: false })
    me.resume()
  })

  this._fst.on('error', function(err) {
    me.emit('error', err)
  })

  this._fst.on('drain', function() {
    me.emit('drain')
  })

  // this._fst.on("end", function () {
  //   console.error("\nEEEE Extract End", me._fst.path)
  // })

  this._fst.on("close", function () {
    // console.error("\nEEEE Extract End", me._fst.path)
    me.emit("finish")
    me.emit("end")
    me.emit("close")
  })
}
```
- example usage
```shell
...
This only works with directories, it does not work with individual files.

The optional 'properties' object are used to set properties in the tar
'Global Extended Header'. If the 'fromBase' property is set to true,
the tar will contain files relative to the path passed, and not with
the path included.

### tar.Extract([options])

Returns a through stream. Write tar data to the stream and the files
in the tarball will be extracted onto the filesystem.

'options' can be:

'''js
...
```

#### <a name="apidoc.element.tar.Pack"></a>[function <span class="apidocSignatureSpan">tar.</span>Pack (props)](#apidoc.element.tar.Pack)
- description and source-code
```javascript
function Pack(props) {
  // console.error("-- p ctor")
  var me = this
  if (!(me instanceof Pack)) return new Pack(props)

  if (props) me._noProprietary = props.noProprietary
  else me._noProprietary = false

  me._global = props

  me.readable = true
  me.writable = true
  me._buffer = []
  // console.error("-- -- set current to null in ctor")
  me._currentEntry = null
  me._processing = false

  me._pipeRoot = null
  me.on("pipe", function (src) {
    if (src.root === me._pipeRoot) return
    me._pipeRoot = src
    src.on("end", function () {
      me._pipeRoot = null
    })
    me.add(src)
  })
}
```
- example usage
```shell
...

See 'examples/' for usage examples.

### var tar = require('tar')

Returns an object with '.Pack', '.Extract' and '.Parse' methods.

### tar.Pack([properties])

Returns a through stream. Use
[fstream](https://npmjs.org/package/fstream) to write files into the
pack stream and you will receive tar archive data from the pack
stream.

This only works with directories, it does not work with individual files.
...
```

#### <a name="apidoc.element.tar.Parse"></a>[function <span class="apidocSignatureSpan">tar.</span>Parse ()](#apidoc.element.tar.Parse)
- description and source-code
```javascript
function Parse() {
  var me = this
  if (!(me instanceof Parse)) return new Parse()

  // doesn't apply fstream.Reader ctor?
  // no, becasue we don't want to stat/etc, we just
  // want to get the entry/add logic from .pipe()
  Stream.apply(me)

  me.writable = true
  me.readable = true
  me._stream = new BlockStream(512)
  me.position = 0
  me._ended = false

  me._stream.on("error", function (e) {
    me.emit("error", e)
  })

  me._stream.on("data", function (c) {
    me._process(c)
  })

  me._stream.on("end", function () {
    me._streamEnd()
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })
}
```
- example usage
```shell
...
  strip: 0, // how many path segments to strip from the root when extracting
}
'''

'options' also get passed to the 'fstream.Writer' instance that 'tar'
uses internally.

### tar.Parse()

Returns a writable stream. Write tar data to it and it will emit
'entry' events for each entry parsed from the tarball. This is used by
'tar.Extract'.
...
```

#### <a name="apidoc.element.tar.Parse.super_"></a>[function <span class="apidocSignatureSpan">tar.</span>Parse.super_ (props, currentStat)](#apidoc.element.tar.Parse.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.buffer_entry"></a>[function <span class="apidocSignatureSpan">tar.</span>buffer_entry ()](#apidoc.element.tar.buffer_entry)
- description and source-code
```javascript
function BufferEntry() {
  Entry.apply(this, arguments)
  this._buffer = new Buffer(this.props.size)
  this._offset = 0
  this.body = ""
  this.on("end", function () {
    this.body = this._buffer.toString().slice(0, -1)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry"></a>[function <span class="apidocSignatureSpan">tar.</span>entry (header, extended, global)](#apidoc.element.tar.entry)
- description and source-code
```javascript
function Entry(header, extended, global) {
  Stream.call(this)
  this.readable = true
  this.writable = true

  this._needDrain = false
  this._paused = false
  this._reading = false
  this._ending = false
  this._ended = false
  this._remaining = 0
  this._abort = false
  this._queue = []
  this._index = 0
  this._queueLen = 0

  this._read = this._read.bind(this)

  this.props = {}
  this._header = header
  this._extended = extended || {}

  // globals can change throughout the course of
  // a file parse operation.  Freeze it at its current state.
  this._global = {}
  var me = this
  Object.keys(global || {}).forEach(function (g) {
    me._global[g] = global[g]
  })

  this._setProps()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>entry_writer (props)](#apidoc.element.tar.entry_writer)
- description and source-code
```javascript
function EntryWriter(props) {
  var me = this

  if (!(me instanceof EntryWriter)) {
    return new EntryWriter(props)
  }

  Stream.apply(this)

  me.writable = true
  me.readable = true

  me._stream = new BlockStream(512)

  me._stream.on("data", function (c) {
    me.emit("data", c)
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })

  me._stream.on("end", function () {
    me.emit("end")
    me.emit("close")
  })

  me.props = props
  if (props.type === "Directory") {
    props.size = 0
  }
  props.ustar = "ustar\0"
  props.ustarver = "00"
  me.path = props.path

  me._buffer = []
  me._didHeader = false
  me._meta = false

  me.on("pipe", function () {
    me._process()
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.extended_header"></a>[function <span class="apidocSignatureSpan">tar.</span>extended_header ()](#apidoc.element.tar.extended_header)
- description and source-code
```javascript
function ExtendedHeader() {
  Entry.apply(this, arguments)
  this.on("data", this._parse)
  this.fields = {}
  this._position = 0
  this._fieldPos = 0
  this._state = SIZE
  this._sizeBuf = []
  this._keyBuf = []
  this._valBuf = []
  this._size = -1
  this._key = ""
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.extended_header_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>extended_header_writer (props)](#apidoc.element.tar.extended_header_writer)
- description and source-code
```javascript
function ExtendedHeaderWriter(props) {
  // console.error(">> ehw ctor")
  var me = this

  if (!(me instanceof ExtendedHeaderWriter)) {
    return new ExtendedHeaderWriter(props)
  }

  me.fields = props

  var p =
    { path : ("PaxHeader" + path.join("/", props.path || ""))
             .replace(/\\/g, "/").substr(0, 100)
    , mode : props.mode || 0666
    , uid : props.uid || 0
    , gid : props.gid || 0
    , size : 0 // will be set later
    , mtime : props.mtime || Date.now() / 1000
    , type : "x"
    , linkpath : ""
    , ustar : "ustar\0"
    , ustarver : "00"
    , uname : props.uname || ""
    , gname : props.gname || ""
    , devmaj : props.devmaj || 0
    , devmin : props.devmin || 0
    }


  EntryWriter.call(me, p)
  // console.error(">> ehw props", me.props)
  me.props = p

  me._meta = true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.global_header_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>global_header_writer (props)](#apidoc.element.tar.global_header_writer)
- description and source-code
```javascript
function GlobalHeaderWriter(props) {
  if (!(this instanceof GlobalHeaderWriter)) {
    return new GlobalHeaderWriter(props)
  }
  ExtendedHeaderWriter.call(this, props)
  this.props.type = "g"
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.header"></a>[function <span class="apidocSignatureSpan">tar.</span>header (block)](#apidoc.element.tar.header)
- description and source-code
```javascript
function TarHeader(block) {
  if (!(this instanceof TarHeader)) return new TarHeader(block)
  if (block) this.decode(block)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Extract"></a>[module tar.Extract](#apidoc.module.tar.Extract)

#### <a name="apidoc.element.tar.Extract.Extract"></a>[function <span class="apidocSignatureSpan">tar.</span>Extract (opts)](#apidoc.element.tar.Extract.Extract)
- description and source-code
```javascript
function Extract(opts) {
  if (!(this instanceof Extract)) return new Extract(opts)
  tar.Parse.apply(this)

  if (typeof opts !== "object") {
    opts = { path: opts }
  }

  // better to drop in cwd? seems more standard.
  opts.path = opts.path || path.resolve("node-tar-extract")
  opts.type = "Directory"
  opts.Directory = true

  // similar to --strip or --strip-components
  opts.strip = +opts.strip
  if (!opts.strip || opts.strip <= 0) opts.strip = 0

  this._fst = fstream.Writer(opts)

  this.pause()
  var me = this

  // Hardlinks in tarballs are relative to the root
  // of the tarball.  So, they need to be resolved against
  // the target directory in order to be created properly.
  me.on("entry", function (entry) {
    // if there's a "strip" argument, then strip off that many
    // path components.
    if (opts.strip) {
      var p = entry.path.split("/").slice(opts.strip).join("/")
      entry.path = entry.props.path = p
      if (entry.linkpath) {
        var lp = entry.linkpath.split("/").slice(opts.strip).join("/")
        entry.linkpath = entry.props.linkpath = lp
      }
    }
    if (entry.type === "Link") {
      entry.linkpath = entry.props.linkpath =
        path.join(opts.path, path.join("/", entry.props.linkpath))
    }

    if (entry.type === "SymbolicLink") {
      var dn = path.dirname(entry.path) || ""
      var linkpath = entry.props.linkpath
      var target = path.resolve(opts.path, dn, linkpath)
      if (target.indexOf(opts.path) !== 0) {
        linkpath = path.join(opts.path, path.join("/", linkpath))
      }
      entry.linkpath = entry.props.linkpath = linkpath
    }
  })

  this._fst.on("ready", function () {
    me.pipe(me._fst, { end: false })
    me.resume()
  })

  this._fst.on('error', function(err) {
    me.emit('error', err)
  })

  this._fst.on('drain', function() {
    me.emit('drain')
  })

  // this._fst.on("end", function () {
  //   console.error("\nEEEE Extract End", me._fst.path)
  // })

  this._fst.on("close", function () {
    // console.error("\nEEEE Extract End", me._fst.path)
    me.emit("finish")
    me.emit("end")
    me.emit("close")
  })
}
```
- example usage
```shell
...
This only works with directories, it does not work with individual files.

The optional 'properties' object are used to set properties in the tar
'Global Extended Header'. If the 'fromBase' property is set to true,
the tar will contain files relative to the path passed, and not with
the path included.

### tar.Extract([options])

Returns a through stream. Write tar data to the stream and the files
in the tarball will be extracted onto the filesystem.

'options' can be:

'''js
...
```

#### <a name="apidoc.element.tar.Extract.super_"></a>[function <span class="apidocSignatureSpan">tar.Extract.</span>super_ ()](#apidoc.element.tar.Extract.super_)
- description and source-code
```javascript
function Parse() {
  var me = this
  if (!(me instanceof Parse)) return new Parse()

  // doesn't apply fstream.Reader ctor?
  // no, becasue we don't want to stat/etc, we just
  // want to get the entry/add logic from .pipe()
  Stream.apply(me)

  me.writable = true
  me.readable = true
  me._stream = new BlockStream(512)
  me.position = 0
  me._ended = false

  me._stream.on("error", function (e) {
    me.emit("error", e)
  })

  me._stream.on("data", function (c) {
    me._process(c)
  })

  me._stream.on("end", function () {
    me._streamEnd()
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Extract.prototype"></a>[module tar.Extract.prototype](#apidoc.module.tar.Extract.prototype)

#### <a name="apidoc.element.tar.Extract.prototype._streamEnd"></a>[function <span class="apidocSignatureSpan">tar.Extract.prototype.</span>_streamEnd ()](#apidoc.element.tar.Extract.prototype._streamEnd)
- description and source-code
```javascript
_streamEnd = function () {
  var me = this
  if (!me._ended || me._entry) me.error("unexpected eof")
  me._fst.end()
  // my .end() is coming later.
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Pack"></a>[module tar.Pack](#apidoc.module.tar.Pack)

#### <a name="apidoc.element.tar.Pack.Pack"></a>[function <span class="apidocSignatureSpan">tar.</span>Pack (props)](#apidoc.element.tar.Pack.Pack)
- description and source-code
```javascript
function Pack(props) {
  // console.error("-- p ctor")
  var me = this
  if (!(me instanceof Pack)) return new Pack(props)

  if (props) me._noProprietary = props.noProprietary
  else me._noProprietary = false

  me._global = props

  me.readable = true
  me.writable = true
  me._buffer = []
  // console.error("-- -- set current to null in ctor")
  me._currentEntry = null
  me._processing = false

  me._pipeRoot = null
  me.on("pipe", function (src) {
    if (src.root === me._pipeRoot) return
    me._pipeRoot = src
    src.on("end", function () {
      me._pipeRoot = null
    })
    me.add(src)
  })
}
```
- example usage
```shell
...

See 'examples/' for usage examples.

### var tar = require('tar')

Returns an object with '.Pack', '.Extract' and '.Parse' methods.

### tar.Pack([properties])

Returns a through stream. Use
[fstream](https://npmjs.org/package/fstream) to write files into the
pack stream and you will receive tar archive data from the pack
stream.

This only works with directories, it does not work with individual files.
...
```

#### <a name="apidoc.element.tar.Pack.super_"></a>[function <span class="apidocSignatureSpan">tar.Pack.</span>super_ ()](#apidoc.element.tar.Pack.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Pack.prototype"></a>[module tar.Pack.prototype](#apidoc.module.tar.Pack.prototype)

#### <a name="apidoc.element.tar.Pack.prototype._process"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>_process ()](#apidoc.element.tar.Pack.prototype._process)
- description and source-code
```javascript
_process = function () {
  var me = this
  if (me._paused || me._processing) {
    return
  }

  var entry = me._buffer.shift()

  if (!entry) {
    if (me._needDrain) {
      me.emit("drain")
    }
    return
  }

  if (entry.ready === false) {
    // console.error("-- entry is not ready", entry)
    me._buffer.unshift(entry)
    entry.on("ready", function () {
      // console.error("-- -- ready!", entry)
      me._process()
    })
    return
  }

  me._processing = true

  if (entry === eof) {
    // need 2 ending null blocks.
    me.emit("data", eof)
    me.emit("data", eof)
    me.emit("end")
    me.emit("close")
    return
  }

  // Change the path to be relative to the root dir that was
  // added to the tarball.
  //
  // XXX This should be more like how -C works, so you can
  // explicitly set a root dir, and also explicitly set a pathname
  // in the tarball to use.  That way we can skip a lot of extra
  // work when resolving symlinks for bundled dependencies in npm.

  var root = path.dirname((entry.root || entry).path);
  if (me._global && me._global.fromBase && entry.root && entry.root.path) {
    // user set 'fromBase: true' indicating tar root should be directory itself
    root = entry.root.path;
  }

  var wprops = {}

  Object.keys(entry.props || {}).forEach(function (k) {
    wprops[k] = entry.props[k]
  })

  if (me._noProprietary) wprops.noProprietary = true

  wprops.path = path.relative(root, entry.path || '')

  // actually not a matter of opinion or taste.
  if (process.platform === "win32") {
    wprops.path = wprops.path.replace(/\\/g, "/")
  }

  if (!wprops.type)
    wprops.type = 'Directory'

  switch (wprops.type) {
    // sockets not supported
    case "Socket":
      return

    case "Directory":
      wprops.path += "/"
      wprops.size = 0
      break

    case "Link":
      var lp = path.resolve(path.dirname(entry.path), entry.linkpath)
      wprops.linkpath = path.relative(root, lp) || "."
      wprops.size = 0
      break

    case "SymbolicLink":
      var lp = path.resolve(path.dirname(entry.path), entry.linkpath)
      wprops.linkpath = path.relative(path.dirname(entry.path), lp) || "."
      wprops.size = 0
      break
  }

  // console.error("-- new writer", wprops)
  // if (!wprops.type) {
  //   // console.error("-- no type?", entry.constructor.name, entry)
  // }

  // console.error("-- -- set current to new writer", wprops.path)
  var writer = me._currentEntry = EntryWriter(wprops)

  writer.parent = me

  // writer.on("end", function () {
  //   // console.error("-- -- writer end", writer.path)
  // })

  writer.on("data", function (c) {
    me.emit("data", c)
  })

  writer.on("header", function () {
    Buffer.prototype.toJSON = function () {
      return this.toString().split(/\0/).join(".")
    }
    // console.error("-- -- writer header %j", writer.props)
    if (writer.props.size === 0) nextEntry()
  })
  writer.on("close", nextEntry)

  var ended = false
  function nextEntry () {
    if (ended) return
    ended = true

    // console.error("-- -- writer close", writer.path)
    // console.error("-- -- set current to null", wprops.path)
    me._currentEntry = null
    me._processing = false
    me._process()
  }

  writer.on("error", function (er) {
    // console.error("-- -- writer error", writer.path)
    me.emit("error", er)
  })

  // if it's the root, then there's no need to add its entries,
  // or data, since they'll be added directly.
  if (entry === me._pipeRoot) {
    // console.error("-- is the root, don't auto-add")
    writer.add = null
  }

  entry.pipe(writer)
}
```
- example usage
```shell
...
me.path = props.path

me._buffer = []
me._didHeader = false
me._meta = false

me.on("pipe", function () {
  me._process()
})
}

EntryWriter.prototype.write = function (c) {
// console.error(".. ew write")
if (this._ended) return this.emit("error", new Error("write after end"))
this._buffer.push(c)
...
```

#### <a name="apidoc.element.tar.Pack.prototype.add"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>add (stream)](#apidoc.element.tar.Pack.prototype.add)
- description and source-code
```javascript
add = function (stream) {
  if (this._global && !this._didGlobal) this.addGlobal(this._global)

  if (this._ended) return this.emit("error", new Error("add after end"))

  collect(stream)
  this._buffer.push(stream)
  this._process()
  this._needDrain = this._buffer.length > 0
  return !this._needDrain
}
```
- example usage
```shell
...
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
this._didHeader = true
...
```

#### <a name="apidoc.element.tar.Pack.prototype.addGlobal"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>addGlobal (props)](#apidoc.element.tar.Pack.prototype.addGlobal)
- description and source-code
```javascript
addGlobal = function (props) {
  // console.error("-- p addGlobal")
  if (this._didGlobal) return
  this._didGlobal = true

  var me = this
  GlobalHeaderWriter(props)
    .on("data", function (c) {
      me.emit("data", c)
    })
    .end()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Pack.prototype.destroy"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>destroy ()](#apidoc.element.tar.Pack.prototype.destroy)
- description and source-code
```javascript
destroy = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Pack.prototype.end"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>end ()](#apidoc.element.tar.Pack.prototype.end)
- description and source-code
```javascript
end = function () {
  this._ended = true
  this._buffer.push(eof)
  this._process()
}
```
- example usage
```shell
...

EntryWriter.prototype.add = function (entry) {
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
...
```

#### <a name="apidoc.element.tar.Pack.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>pause ()](#apidoc.element.tar.Pack.prototype.pause)
- description and source-code
```javascript
pause = function () {
  this._paused = true
  if (this._currentEntry) this._currentEntry.pause()
  this.emit("pause")
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Pack.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>resume ()](#apidoc.element.tar.Pack.prototype.resume)
- description and source-code
```javascript
resume = function () {
  this._paused = false
  if (this._currentEntry) this._currentEntry.resume()
  this.emit("resume")
  this._process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Pack.prototype.write"></a>[function <span class="apidocSignatureSpan">tar.Pack.prototype.</span>write ()](#apidoc.element.tar.Pack.prototype.write)
- description and source-code
```javascript
write = function () {}
```
- example usage
```shell
...
  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
// console.error(".. .. .. i=%d", i)

var c = buf[i]

if (c === EOF) this._stream.end()
else this._stream.write(c)

if (this._paused) {
  // console.error(".. .. .. paused mid-emission")
  this._processing = false
  if (i < buf.length) {
    this._needDrain = true
    this._buffer = buf.slice(i + 1)
...
```



# <a name="apidoc.module.tar.Parse"></a>[module tar.Parse](#apidoc.module.tar.Parse)

#### <a name="apidoc.element.tar.Parse.Parse"></a>[function <span class="apidocSignatureSpan">tar.</span>Parse ()](#apidoc.element.tar.Parse.Parse)
- description and source-code
```javascript
function Parse() {
  var me = this
  if (!(me instanceof Parse)) return new Parse()

  // doesn't apply fstream.Reader ctor?
  // no, becasue we don't want to stat/etc, we just
  // want to get the entry/add logic from .pipe()
  Stream.apply(me)

  me.writable = true
  me.readable = true
  me._stream = new BlockStream(512)
  me.position = 0
  me._ended = false

  me._stream.on("error", function (e) {
    me.emit("error", e)
  })

  me._stream.on("data", function (c) {
    me._process(c)
  })

  me._stream.on("end", function () {
    me._streamEnd()
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })
}
```
- example usage
```shell
...
  strip: 0, // how many path segments to strip from the root when extracting
}
'''

'options' also get passed to the 'fstream.Writer' instance that 'tar'
uses internally.

### tar.Parse()

Returns a writable stream. Write tar data to it and it will emit
'entry' events for each entry parsed from the tarball. This is used by
'tar.Extract'.
...
```

#### <a name="apidoc.element.tar.Parse.create"></a>[function <span class="apidocSignatureSpan">tar.Parse.</span>create ()](#apidoc.element.tar.Parse.create)
- description and source-code
```javascript
function Parse() {
  var me = this
  if (!(me instanceof Parse)) return new Parse()

  // doesn't apply fstream.Reader ctor?
  // no, becasue we don't want to stat/etc, we just
  // want to get the entry/add logic from .pipe()
  Stream.apply(me)

  me.writable = true
  me.readable = true
  me._stream = new BlockStream(512)
  me.position = 0
  me._ended = false

  me._stream.on("error", function (e) {
    me.emit("error", e)
  })

  me._stream.on("data", function (c) {
    me._process(c)
  })

  me._stream.on("end", function () {
    me._streamEnd()
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_"></a>[function <span class="apidocSignatureSpan">tar.Parse.</span>super_ (props, currentStat)](#apidoc.element.tar.Parse.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.prototype"></a>[module tar.Parse.prototype](#apidoc.module.tar.Parse.prototype)

#### <a name="apidoc.element.tar.Parse.prototype._process"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_process (c)](#apidoc.element.tar.Parse.prototype._process)
- description and source-code
```javascript
_process = function (c) {
  assert(c && c.length === 512, "block size should be 512")

  // one of three cases.
  // 1. A new header
  // 2. A part of a file/extended header
  // 3. One of two or more EOF null blocks

  if (this._entry) {
    var entry = this._entry
    if(!entry._abort) entry.write(c)
    else {
      entry._remaining -= c.length
      if(entry._remaining < 0) entry._remaining = 0
    }
    if (entry._remaining === 0) {
      entry.end()
      this._entry = null
    }
  } else {
    // either zeroes or a header
    var zero = true
    for (var i = 0; i < 512 && zero; i ++) {
      zero = c[i] === 0
    }

    // eof is *at least* 2 blocks of nulls, and then the end of the
    // file.  you can put blocks of nulls between entries anywhere,
    // so appending one tarball to another is technically valid.
    // ending without the eof null blocks is not allowed, however.
    if (zero) {
      if (this._eofStarted)
        this._ended = true
      this._eofStarted = true
    } else {
      this._eofStarted = false
      this._startEntry(c)
    }
  }

  this.position += 512
}
```
- example usage
```shell
...
me.path = props.path

me._buffer = []
me._didHeader = false
me._meta = false

me.on("pipe", function () {
  me._process()
})
}

EntryWriter.prototype.write = function (c) {
// console.error(".. ew write")
if (this._ended) return this.emit("error", new Error("write after end"))
this._buffer.push(c)
...
```

#### <a name="apidoc.element.tar.Parse.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_read ()](#apidoc.element.tar.Parse.prototype._read)
- description and source-code
```javascript
_read = function () {}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.Parse.prototype._startEntry"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_startEntry (c)](#apidoc.element.tar.Parse.prototype._startEntry)
- description and source-code
```javascript
_startEntry = function (c) {
  var header = new TarHeader(c)
    , self = this
    , entry
    , ev
    , EntryType
    , onend
    , meta = false

  if (null === header.size || !header.cksumValid) {
    var e = new Error("invalid tar file")
    e.header = header
    e.tar_file_offset = this.position
    e.tar_block = this.position / 512
    return this.emit("error", e)
  }

  switch (tar.types[header.type]) {
    case "File":
    case "OldFile":
    case "Link":
    case "SymbolicLink":
    case "CharacterDevice":
    case "BlockDevice":
    case "Directory":
    case "FIFO":
    case "ContiguousFile":
    case "GNUDumpDir":
      // start a file.
      // pass in any extended headers
      // These ones consumers are typically most interested in.
      EntryType = Entry
      ev = "entry"
      break

    case "GlobalExtendedHeader":
      // extended headers that apply to the rest of the tarball
      EntryType = ExtendedHeader
      onend = function () {
        self._global = self._global || {}
        Object.keys(entry.fields).forEach(function (k) {
          self._global[k] = entry.fields[k]
        })
      }
      ev = "globalExtendedHeader"
      meta = true
      break

    case "ExtendedHeader":
    case "OldExtendedHeader":
      // extended headers that apply to the next entry
      EntryType = ExtendedHeader
      onend = function () {
        self._extended = entry.fields
      }
      ev = "extendedHeader"
      meta = true
      break

    case "NextFileHasLongLinkpath":
      // set linkpath=<contents> in extended header
      EntryType = BufferEntry
      onend = function () {
        self._extended = self._extended || {}
        self._extended.linkpath = entry.body
      }
      ev = "longLinkpath"
      meta = true
      break

    case "NextFileHasLongPath":
    case "OldGnuLongPath":
      // set path=<contents> in file-extended header
      EntryType = BufferEntry
      onend = function () {
        self._extended = self._extended || {}
        self._extended.path = entry.body
      }
      ev = "longPath"
      meta = true
      break

    default:
      // all the rest we skip, but still set the _entry
      // member, so that we can skip over their data appropriately.
      // emit an event to say that this is an ignored entry type?
      EntryType = Entry
      ev = "ignoredEntry"
      break
  }

  var global, extended
  if (meta) {
    global = extended = null
  } else {
    var global = this._global
    var extended = this._extended

    // extendedHeader only applies to one entry, so once we start
    // an entry, it's over.
    this._extended = null
  }
  entry = new EntryType(header, extended, global)
  entry.meta = meta

  // only proxy data events of normal files.
  if (!meta) {
    entry.on("data", function (c) {
      me.emit("data", c)
    })
  }

  if (onend) entry.on("end", onend)

  this._entry = entry
  var me = this

  entry.on("pause", function () {
    me.pause()
  })

  entry.on("resume", function () {
    me.resume()
  })

  if (this.listeners("*").length) {
    this.emit("*", ev, entry)
  }

  this.emit(ev, entry)

  // Zero-byte entry.  End immediately.
  if (entry.props.size === 0) {
    entry.end()
    this._entry = null
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.prototype._streamEnd"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>_streamEnd ()](#apidoc.element.tar.Parse.prototype._streamEnd)
- description and source-code
```javascript
_streamEnd = function () {
  var me = this
  if (!me._ended || me._entry) me.error("unexpected eof")
  me.emit("end")
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.prototype.end"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>end (c)](#apidoc.element.tar.Parse.prototype.end)
- description and source-code
```javascript
end = function (c) {
  this._ended = true
  return this._stream.end(c)
}
```
- example usage
```shell
...

EntryWriter.prototype.add = function (entry) {
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
...
```

#### <a name="apidoc.element.tar.Parse.prototype.write"></a>[function <span class="apidocSignatureSpan">tar.Parse.prototype.</span>write (c)](#apidoc.element.tar.Parse.prototype.write)
- description and source-code
```javascript
write = function (c) {
  if (this._ended) {
    // gnutar puts a LOT of nulls at the end.
    // you can keep writing these things forever.
    // Just ignore them.
    for (var i = 0, l = c.length; i > l; i ++) {
      if (c[i] !== 0) return this.error("write() after end()")
    }
    return
  }
  return this._stream.write(c)
}
```
- example usage
```shell
...
  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
// console.error(".. .. .. i=%d", i)

var c = buf[i]

if (c === EOF) this._stream.end()
else this._stream.write(c)

if (this._paused) {
  // console.error(".. .. .. paused mid-emission")
  this._processing = false
  if (i < buf.length) {
    this._needDrain = true
    this._buffer = buf.slice(i + 1)
...
```



# <a name="apidoc.module.tar.Parse.super_"></a>[module tar.Parse.super_](#apidoc.module.tar.Parse.super_)

#### <a name="apidoc.element.tar.Parse.super_.super_"></a>[function <span class="apidocSignatureSpan">tar.Parse.</span>super_ ()](#apidoc.element.tar.Parse.super_.super_)
- description and source-code
```javascript
function Abstract() {
  Stream.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Dir (props)](#apidoc.element.tar.Parse.super_.Dir)
- description and source-code
```javascript
function DirReader(props) {
  var self = this
  if (!(self instanceof DirReader)) {
    throw new Error('DirReader must be called as constructor.')
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    throw new Error('Non-directory type ' + props.type)
  }

  self.entries = null
  self._index = -1
  self._paused = false
  self._length = -1

  if (props.sort) {
    this.sort = props.sort
  }

  Reader.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.File"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.</span>File (props)](#apidoc.element.tar.Parse.super_.File)
- description and source-code
```javascript
function FileReader(props) {
  // console.error("    FR create", props.path, props.size, new Error().stack)
  var self = this
  if (!(self instanceof FileReader)) {
    throw new Error('FileReader must be called as constructor.')
  }

  // should already be established as a File type
  // XXX Todo: preserve hardlinks by tracking dev+inode+nlink,
  // with a HardLinkReader class.
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'File' && props.File))) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesEmitted = 0
  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Link"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Link (props)](#apidoc.element.tar.Parse.super_.Link)
- description and source-code
```javascript
function LinkReader(props) {
  var self = this
  if (!(self instanceof LinkReader)) {
    throw new Error('LinkReader must be called as constructor.')
  }

  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Proxy"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.</span>Proxy (props)](#apidoc.element.tar.Parse.super_.Proxy)
- description and source-code
```javascript
function ProxyReader(props) {
  var self = this
  if (!(self instanceof ProxyReader)) {
    throw new Error('ProxyReader must be called as constructor.')
  }

  self.props = props
  self._buffer = []
  self.ready = false

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.Dir.prototype"></a>[module tar.Parse.super_.Dir.prototype](#apidoc.module.tar.Parse.super_.Dir.prototype)

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype._getEntries"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>_getEntries ()](#apidoc.element.tar.Parse.super_.Dir.prototype._getEntries)
- description and source-code
```javascript
_getEntries = function () {
  var self = this

  // race condition.  might pause() before calling _getEntries,
  // and then resume, and try to get them a second time.
  if (self._gotEntries) return
  self._gotEntries = true

  fs.readdir(self._path, function (er, entries) {
    if (er) return self.error(er)

    self.entries = entries

    self.emit('entries', entries)
    if (self._paused) self.once('resume', processEntries)
    else processEntries()

    function processEntries () {
      self._length = self.entries.length
      if (typeof self.sort === 'function') {
        self.entries = self.entries.sort(self.sort.bind(self))
      }
      self._read()
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.Dir.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this

  if (!self.entries) return self._getEntries()

  if (self._paused || self._currentEntry || self._aborted) {
    // console.error('DR paused=%j, current=%j, aborted=%j', self._paused, !!self._currentEntry, self._aborted)
    return
  }

  self._index++
  if (self._index >= self.entries.length) {
    if (!self._ended) {
      self._ended = true
      self.emit('end')
      self.emit('close')
    }
    return
  }

  // ok, handle this one, then.

  // save creating a proxy, by stat'ing the thing now.
  var p = path.resolve(self._path, self.entries[self._index])
  assert(p !== self._path)
  assert(self.entries[self._index])

  // set this to prevent trying to _read() again in the stat time.
  self._currentEntry = p
  fs[ self.props.follow ? 'stat' : 'lstat' ](p, function (er, stat) {
    if (er) return self.error(er)

    var who = self._proxy || self

    stat.path = p
    stat.basename = path.basename(p)
    stat.dirname = path.dirname(p)
    var childProps = self.getChildProps.call(who, stat)
    childProps.path = p
    childProps.basename = path.basename(p)
    childProps.dirname = path.dirname(p)

    var entry = Reader(childProps, stat)

    // console.error("DR Entry", p, stat.size)

    self._currentEntry = entry

    // "entry" events are for direct entries in a specific dir.
    // "child" events are for any and all children at all levels.
    // This nomenclature is not completely final.

    entry.on('pause', function (who) {
      if (!self._paused && !entry._disowned) {
        self.pause(who)
      }
    })

    entry.on('resume', function (who) {
      if (self._paused && !entry._disowned) {
        self.resume(who)
      }
    })

    entry.on('stat', function (props) {
      self.emit('_entryStat', entry, props)
      if (entry._aborted) return
      if (entry._paused) {
        entry.once('resume', function () {
          self.emit('entryStat', entry, props)
        })
      } else self.emit('entryStat', entry, props)
    })

    entry.on('ready', function EMITCHILD () {
      // console.error("DR emit child", entry._path)
      if (self._paused) {
        // console.error("  DR emit child - try again later")
        // pause the child, and emit the "entry" event once we drain.
        // console.error("DR pausing child entry")
        entry.pause(self)
        return self.once('resume', EMITCHILD)
      }

      // skip over sockets.  they can't be piped around properly,
      // so there's really no sense even acknowledging them.
      // if someone really wants to see them, they can listen to
      // the "socket" events.
      if (entry.type === 'Socket') {
        self.emit('socket', entry)
      } else {
        self.emitEntry(entry)
      }
    })

    var ended = false
    entry.on('close', onend)
    entry.on('disown', onend)
    function onend () {
      if (ended) return
      ended = true
      self.emit('childEnd', entry)
      self.emit('entryEnd', entry)
      self._currentEntry = null
      if (!self._paused) {
        self._read()
      }
    }

    // XXX Remove this.  Works in node as of 0.6.2 or so.
    // Long filenames should not break stuff.
    entry.on('error', function (er) {
      if (entry._swallowErrors) {
        self.warn(er)
        entry.emit('end')
        entry.emit('close')
      } else {
        self.emit('error', er)
      }
    })

    // proxy up some events.
    ;[
      'child',
      'childEnd',
      'warn'
    ].forEach(function (ev) {
      entry.on(ev, self.emit.bind(self, ev))
    })
  })
}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype.disown"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>disown (entry)](#apidoc.element.tar.Parse.super_.Dir.prototype.disown)
- description and source-code
```javascript
disown = function (entry) {
  entry.emit('beforeDisown')
  entry._disowned = true
  entry.parent = entry.root = null
  if (entry === this._currentEntry) {
    this._currentEntry = null
  }
  entry.emit('disown')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype.emitEntry"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>emitEntry (entry)](#apidoc.element.tar.Parse.super_.Dir.prototype.emitEntry)
- description and source-code
```javascript
emitEntry = function (entry) {
  this.emit('entry', entry)
  this.emit('child', entry)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype.getChildProps"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>getChildProps ()](#apidoc.element.tar.Parse.super_.Dir.prototype.getChildProps)
- description and source-code
```javascript
getChildProps = function () {
  return {
    depth: this.depth + 1,
    root: this.root || this,
    parent: this,
    follow: this.follow,
    filter: this.filter,
    sort: this.props.sort,
    hardlinks: this.props.hardlinks
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.Dir.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  var self = this
  if (self._paused) return
  who = who || self
  self._paused = true
  if (self._currentEntry && self._currentEntry.pause) {
    self._currentEntry.pause(who)
  }
  self.emit('pause', who)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Dir.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Dir.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.Dir.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  var self = this
  if (!self._paused) return
  who = who || self

  self._paused = false
  // console.error('DR Emit Resume', self._path)
  self.emit('resume', who)
  if (self._paused) {
    // console.error('DR Re-paused', self._path)
    return
  }

  if (self._currentEntry) {
    if (self._currentEntry.resume) self._currentEntry.resume(who)
  } else self._read()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.File.prototype"></a>[module tar.Parse.super_.File.prototype](#apidoc.module.tar.Parse.super_.File.prototype)

#### <a name="apidoc.element.tar.Parse.super_.File.prototype._getStream"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>_getStream ()](#apidoc.element.tar.Parse.super_.File.prototype._getStream)
- description and source-code
```javascript
_getStream = function () {
  var self = this
  var stream = self._stream = fs.createReadStream(self._path, self.props)

  if (self.props.blksize) {
    stream.bufferSize = self.props.blksize
  }

  stream.on('open', self.emit.bind(self, 'open'))

  stream.on('data', function (c) {
    // console.error('\t\t%d %s', c.length, self.basename)
    self._bytesEmitted += c.length
    // no point saving empty chunks
    if (!c.length) {
      return
    } else if (self._paused || self._buffer.length) {
      self._buffer.push(c)
      self._read()
    } else self.emit('data', c)
  })

  stream.on('end', function () {
    if (self._paused || self._buffer.length) {
      // console.error('FR Buffering End', self._path)
      self._buffer.push(EOF)
      self._read()
    } else {
      self.emit('end')
    }

    if (self._bytesEmitted !== self.props.size) {
      self.error("Didn't get expected byte count\n" +
        'expect: ' + self.props.size + '\n' +
        'actual: ' + self._bytesEmitted)
    }
  })

  stream.on('close', function () {
    if (self._paused || self._buffer.length) {
      // console.error('FR Buffering Close', self._path)
      self._buffer.push(CLOSE)
      self._read()
    } else {
      // console.error('FR close 1', self._path)
      self.emit('close')
    }
  })

  stream.on('error', function (e) {
    self.emit('error', e)
  })

  self._read()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.File.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.File.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  // console.error('FR _read', self._path)
  if (self._paused) {
    // console.error('FR _read paused', self._path)
    return
  }

  if (!self._stream) {
    // console.error('FR _getStream calling', self._path)
    return self._getStream()
  }

  // clear out the buffer, if there is one.
  if (self._buffer.length) {
    // console.error('FR _read has buffer', self._buffer.length, self._path)
    var buf = self._buffer
    for (var i = 0, l = buf.length; i < l; i++) {
      var c = buf[i]
      if (c === EOF) {
        // console.error('FR Read emitting buffered end', self._path)
        self.emit('end')
      } else if (c === CLOSE) {
        // console.error('FR Read emitting buffered close', self._path)
        self.emit('close')
      } else {
        // console.error('FR Read emitting buffered data', self._path)
        self.emit('data', c)
      }

      if (self._paused) {
        // console.error('FR Read Re-pausing at '+i, self._path)
        self._buffer = buf.slice(i)
        return
      }
    }
    self._buffer.length = 0
  }
// console.error("FR _read done")
// that's about all there is to it.
}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.Parse.super_.File.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.File.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  var self = this
  // console.error('FR Pause', self._path)
  if (self._paused) return
  who = who || self
  self._paused = true
  if (self._stream) self._stream.pause()
  self.emit('pause', who)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.File.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.File.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.File.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  var self = this
  // console.error('FR Resume', self._path)
  if (!self._paused) return
  who = who || self
  self.emit('resume', who)
  self._paused = false
  if (self._stream) self._stream.resume()
  self._read()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.Link.prototype"></a>[module tar.Parse.super_.Link.prototype](#apidoc.module.tar.Parse.super_.Link.prototype)

#### <a name="apidoc.element.tar.Parse.super_.Link.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Link.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.Link.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  if (self._paused) return
  // basically just a no-op, since we got all the info we need
  // from the _stat method
  if (!self._ended) {
    self.emit('end')
    self.emit('close')
    self._ended = true
  }
}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.Parse.super_.Link.prototype._stat"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Link.prototype.</span>_stat (currentStat)](#apidoc.element.tar.Parse.super_.Link.prototype._stat)
- description and source-code
```javascript
_stat = function (currentStat) {
  var self = this
  fs.readlink(self._path, function (er, linkpath) {
    if (er) return self.error(er)
    self.linkpath = self.props.linkpath = linkpath
    self.emit('linkpath', linkpath)
    Reader.prototype._stat.call(self, currentStat)
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.Proxy.prototype"></a>[module tar.Parse.super_.Proxy.prototype](#apidoc.module.tar.Parse.super_.Proxy.prototype)

#### <a name="apidoc.element.tar.Parse.super_.Proxy.prototype._addProxy"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>_addProxy (proxy)](#apidoc.element.tar.Parse.super_.Proxy.prototype._addProxy)
- description and source-code
```javascript
_addProxy = function (proxy) {
  var self = this
  if (self._proxyTarget) {
    return self.error('proxy already set')
  }

  self._proxyTarget = proxy
  proxy._proxy = self

  ;[
    'error',
    'data',
    'end',
    'close',
    'linkpath',
    'entry',
    'entryEnd',
    'child',
    'childEnd',
    'warn',
    'stat'
  ].forEach(function (ev) {
    // console.error('~~ proxy event', ev, self.path)
    proxy.on(ev, self.emit.bind(self, ev))
  })

  self.emit('proxy', proxy)

  proxy.on('ready', function () {
    // console.error("~~ proxy is ready!", self.path)
    self.ready = true
    self.emit('ready')
  })

  var calls = self._buffer
  self._buffer.length = 0
  calls.forEach(function (c) {
    proxy[c[0]].apply(proxy, c[1])
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Proxy.prototype._stat"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>_stat ()](#apidoc.element.tar.Parse.super_.Proxy.prototype._stat)
- description and source-code
```javascript
_stat = function () {
  var self = this
  var props = self.props
  // stat the thing to see what the proxy should be.
  var stat = props.follow ? 'stat' : 'lstat'

  fs[stat](props.path, function (er, current) {
    var type
    if (er || !current) {
      type = 'File'
    } else {
      type = getType(current)
    }

    props[type] = true
    props.type = self.type = type

    self._old = current
    self._addProxy(Reader(props, current))
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Proxy.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>pause ()](#apidoc.element.tar.Parse.super_.Proxy.prototype.pause)
- description and source-code
```javascript
pause = function () {
  return this._proxyTarget ? this._proxyTarget.pause() : false
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.Proxy.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.Proxy.prototype.</span>resume ()](#apidoc.element.tar.Parse.super_.Proxy.prototype.resume)
- description and source-code
```javascript
resume = function () {
  return this._proxyTarget ? this._proxyTarget.resume() : false
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.prototype"></a>[module tar.Parse.super_.prototype](#apidoc.module.tar.Parse.super_.prototype)

#### <a name="apidoc.element.tar.Parse.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>_read ()](#apidoc.element.tar.Parse.super_.prototype._read)
- description and source-code
```javascript
_read = function () {
  this.error('Cannot read unknown type: ' + this.type)
}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.Parse.super_.prototype._stat"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>_stat (currentStat)](#apidoc.element.tar.Parse.super_.prototype._stat)
- description and source-code
```javascript
_stat = function (currentStat) {
  var self = this
  var props = self.props
  var stat = props.follow ? 'stat' : 'lstat'
  // console.error("Reader._stat", self._path, currentStat)
  if (currentStat) process.nextTick(statCb.bind(null, null, currentStat))
  else fs[stat](self._path, statCb)

  function statCb (er, props_) {
    // console.error("Reader._stat, statCb", self._path, props_, props_.nlink)
    if (er) return self.error(er)

    Object.keys(props_).forEach(function (k) {
      props[k] = props_[k]
    })

    // if it's not the expected size, then abort here.
    if (undefined !== self.size && props.size !== self.size) {
      return self.error('incorrect size')
    }
    self.size = props.size

    var type = getType(props)
    var handleHardlinks = props.hardlinks !== false

    // special little thing for handling hardlinks.
    if (handleHardlinks && type !== 'Directory' && props.nlink && props.nlink > 1) {
      var k = props.dev + ':' + props.ino
      // console.error("Reader has nlink", self._path, k)
      if (hardLinks[k] === self._path || !hardLinks[k]) {
        hardLinks[k] = self._path
      } else {
        // switch into hardlink mode.
        type = self.type = self.props.type = 'Link'
        self.Link = self.props.Link = true
        self.linkpath = self.props.linkpath = hardLinks[k]
        // console.error("Hardlink detected, switching mode", self._path, self.linkpath)
        // Setting __proto__ would arguably be the "correct"
        // approach here, but that just seems too wrong.
        self._stat = self._read = LinkReader.prototype._read
      }
    }

    if (self.type && self.type !== type) {
      self.error('Unexpected type: ' + type)
    }

    // if the filter doesn't pass, then just skip over this one.
    // still have to emit end so that dir-walking can move on.
    if (self.filter) {
      var who = self._proxy || self
      // special handling for ProxyReaders
      if (!self.filter.call(who, who, props)) {
        if (!self._disowned) {
          self.abort()
          self.emit('end')
          self.emit('close')
        }
        return
      }
    }

    // last chance to abort or disown before the flow starts!
    var events = ['_stat', 'stat', 'ready']
    var e = 0
    ;(function go () {
      if (self._aborted) {
        self.emit('end')
        self.emit('close')
        return
      }

      if (self._paused && self.type !== 'Directory') {
        self.once('resume', go)
        return
      }

      var ev = events[e++]
      if (!ev) {
        return self._read()
      }
      self.emit(ev, props)
      go()
    })()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>pause (who)](#apidoc.element.tar.Parse.super_.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  this._paused = true
  who = who || this
  this.emit('pause', who)
  if (this._stream) this._stream.pause(who)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>pipe (dest)](#apidoc.element.tar.Parse.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest) {
  var self = this
  if (typeof dest.add === 'function') {
    // piping to a multi-compatible, and we've got directory entries.
    self.on('entry', function (entry) {
      var ret = dest.add(entry)
      if (ret === false) {
        self.pause()
      }
    })
  }

  // console.error("R Pipe apply Stream Pipe")
  return Stream.prototype.pipe.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.prototype.</span>resume (who)](#apidoc.element.tar.Parse.super_.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  this._paused = false
  who = who || this
  this.emit('resume', who)
  if (this._stream) this._stream.resume(who)
  this._read()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.Parse.super_.super_.prototype"></a>[module tar.Parse.super_.super_.prototype](#apidoc.module.tar.Parse.super_.super_.prototype)

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.abort"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>abort ()](#apidoc.element.tar.Parse.super_.super_.prototype.abort)
- description and source-code
```javascript
abort = function () {
  this._aborted = true
  this.emit('abort')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.destroy"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>destroy ()](#apidoc.element.tar.Parse.super_.super_.prototype.destroy)
- description and source-code
```javascript
destroy = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.error"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>error (msg, code, th)](#apidoc.element.tar.Parse.super_.super_.prototype.error)
- description and source-code
```javascript
error = function (msg, code, th) {
  var er = decorate(msg, code, this)
  if (th) throw er
  else this.emit('error', er)
}
```
- example usage
```shell
...

  me.on("pipe", function () {
    me._process()
  })
}

EntryWriter.prototype.write = function (c) {
  // console.error(".. ew write")
  if (this._ended) return this.emit("error", new Error("write after end"))
  this._buffer.push(c)
  this._process()
  this._needDrain = this._buffer.length > 0
  return !this._needDrain
}
...
```

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.info"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>info (msg, code)](#apidoc.element.tar.Parse.super_.super_.prototype.info)
- description and source-code
```javascript
info = function (msg, code) {
  this.emit('info', msg, code)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.tar.Parse.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  if (ev === 'ready' && this.ready) {
    process.nextTick(fn.bind(this))
  } else {
    Stream.prototype.on.call(this, ev, fn)
  }
  return this
}
```
- example usage
```shell
...
  , Entry = require("./entry.js")

function BufferEntry () {
  Entry.apply(this, arguments)
  this._buffer = new Buffer(this.props.size)
  this._offset = 0
  this.body = ""
  this.on("end", function () {
    this.body = this._buffer.toString().slice(0, -1)
  })
}

inherits(BufferEntry, Entry)

// collect the bytes as they come in.
...
```

#### <a name="apidoc.element.tar.Parse.super_.super_.prototype.warn"></a>[function <span class="apidocSignatureSpan">tar.Parse.super_.super_.prototype.</span>warn (msg, code)](#apidoc.element.tar.Parse.super_.super_.prototype.warn)
- description and source-code
```javascript
warn = function (msg, code) {
  var self = this
  var er = decorate(msg, code, self)
  if (!self.listeners('warn')) {
    console.error('%s %s\n' +
    'path = %s\n' +
    'syscall = %s\n' +
    'fstream_type = %s\n' +
    'fstream_path = %s\n' +
    'fstream_unc_path = %s\n' +
    'fstream_class = %s\n' +
    'fstream_stack =\n%s\n',
      code || 'UNKNOWN',
      er.stack,
      er.path,
      er.syscall,
      er.fstream_type,
      er.fstream_path,
      er.fstream_unc_path,
      er.fstream_class,
      er.fstream_stack.join('\n'))
  } else {
    self.emit('warn', er)
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.buffer_entry"></a>[module tar.buffer_entry](#apidoc.module.tar.buffer_entry)

#### <a name="apidoc.element.tar.buffer_entry.buffer_entry"></a>[function <span class="apidocSignatureSpan">tar.</span>buffer_entry ()](#apidoc.element.tar.buffer_entry.buffer_entry)
- description and source-code
```javascript
function BufferEntry() {
  Entry.apply(this, arguments)
  this._buffer = new Buffer(this.props.size)
  this._offset = 0
  this.body = ""
  this.on("end", function () {
    this.body = this._buffer.toString().slice(0, -1)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.buffer_entry.super_"></a>[function <span class="apidocSignatureSpan">tar.buffer_entry.</span>super_ (header, extended, global)](#apidoc.element.tar.buffer_entry.super_)
- description and source-code
```javascript
function Entry(header, extended, global) {
  Stream.call(this)
  this.readable = true
  this.writable = true

  this._needDrain = false
  this._paused = false
  this._reading = false
  this._ending = false
  this._ended = false
  this._remaining = 0
  this._abort = false
  this._queue = []
  this._index = 0
  this._queueLen = 0

  this._read = this._read.bind(this)

  this.props = {}
  this._header = header
  this._extended = extended || {}

  // globals can change throughout the course of
  // a file parse operation.  Freeze it at its current state.
  this._global = {}
  var me = this
  Object.keys(global || {}).forEach(function (g) {
    me._global[g] = global[g]
  })

  this._setProps()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.buffer_entry.prototype"></a>[module tar.buffer_entry.prototype](#apidoc.module.tar.buffer_entry.prototype)

#### <a name="apidoc.element.tar.buffer_entry.prototype.write"></a>[function <span class="apidocSignatureSpan">tar.buffer_entry.prototype.</span>write (c)](#apidoc.element.tar.buffer_entry.prototype.write)
- description and source-code
```javascript
write = function (c) {
  c.copy(this._buffer, this._offset)
  this._offset += c.length
  Entry.prototype.write.call(this, c)
}
```
- example usage
```shell
...
  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
// console.error(".. .. .. i=%d", i)

var c = buf[i]

if (c === EOF) this._stream.end()
else this._stream.write(c)

if (this._paused) {
  // console.error(".. .. .. paused mid-emission")
  this._processing = false
  if (i < buf.length) {
    this._needDrain = true
    this._buffer = buf.slice(i + 1)
...
```



# <a name="apidoc.module.tar.entry"></a>[module tar.entry](#apidoc.module.tar.entry)

#### <a name="apidoc.element.tar.entry.entry"></a>[function <span class="apidocSignatureSpan">tar.</span>entry (header, extended, global)](#apidoc.element.tar.entry.entry)
- description and source-code
```javascript
function Entry(header, extended, global) {
  Stream.call(this)
  this.readable = true
  this.writable = true

  this._needDrain = false
  this._paused = false
  this._reading = false
  this._ending = false
  this._ended = false
  this._remaining = 0
  this._abort = false
  this._queue = []
  this._index = 0
  this._queueLen = 0

  this._read = this._read.bind(this)

  this.props = {}
  this._header = header
  this._extended = extended || {}

  // globals can change throughout the course of
  // a file parse operation.  Freeze it at its current state.
  this._global = {}
  var me = this
  Object.keys(global || {}).forEach(function (g) {
    me._global[g] = global[g]
  })

  this._setProps()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry.super_"></a>[function <span class="apidocSignatureSpan">tar.entry.</span>super_ ()](#apidoc.element.tar.entry.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.entry.prototype"></a>[module tar.entry.prototype](#apidoc.module.tar.entry.prototype)

#### <a name="apidoc.element.tar.entry.prototype._read"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>_read ()](#apidoc.element.tar.entry.prototype._read)
- description and source-code
```javascript
_read = function () {
  // console.error("    Tar Entry _read", this.path)

  if (this._paused || this._reading || this._ended) return

  // set this flag so that event handlers don't inadvertently
  // get multiple _read() calls running.
  this._reading = true

  // have any data to emit?
  while (this._index < this._queueLen && !this._paused) {
    var chunk = this._queue[this._index ++]
    this.emit("data", chunk)
  }

  // check if we're drained
  if (this._index >= this._queueLen) {
    this._queue.length = this._queueLen = this._index = 0
    if (this._needDrain) {
      this._needDrain = false
      this.emit("drain")
    }
    if (this._ending) {
      this._ended = true
      this.emit("end")
    }
  }

  // if the queue gets too big, then pluck off whatever we can.
  // this should be fairly rare.
  var mql = this._maxQueueLen
  if (this._queueLen > mql && this._index > 0) {
    mql = Math.min(this._index, mql)
    this._index -= mql
    this._queueLen -= mql
    this._queue = this._queue.slice(mql)
  }

  this._reading = false
}
```
- example usage
```shell
...
this._remaining -= c.length

// put it on the stack.
var ql = this._queueLen
this._queue.push(c)
this._queueLen ++

this._read()

// either paused, or buffered
if (this._paused || ql > 0) {
  this._needDrain = true
  return false
}
...
```

#### <a name="apidoc.element.tar.entry.prototype._setProps"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>_setProps ()](#apidoc.element.tar.entry.prototype._setProps)
- description and source-code
```javascript
_setProps = function () {
  // props = extended->global->header->{}
  var header = this._header
    , extended = this._extended
    , global = this._global
    , props = this.props

  // first get the values from the normal header.
  var fields = tar.fields
  for (var f = 0; fields[f] !== null; f ++) {
    var field = fields[f]
      , val = header[field]
    if (typeof val !== "undefined") props[field] = val
  }

  // next, the global header for this file.
  // numeric values, etc, will have already been parsed.
  ;[global, extended].forEach(function (p) {
    Object.keys(p).forEach(function (f) {
      if (typeof p[f] !== "undefined") props[f] = p[f]
    })
  })

  // no nulls allowed in path or linkpath
  ;["path", "linkpath"].forEach(function (p) {
    if (props.hasOwnProperty(p)) {
      props[p] = props[p].split("\0")[0]
    }
  })


  // set date fields to be a proper date
  ;["mtime", "ctime", "atime"].forEach(function (p) {
    if (props.hasOwnProperty(p)) {
      props[p] = new Date(props[p] * 1000)
    }
  })

  // set the type so that we know what kind of file to create
  var type
  switch (tar.types[props.type]) {
    case "OldFile":
    case "ContiguousFile":
      type = "File"
      break

    case "GNUDumpDir":
      type = "Directory"
      break

    case undefined:
      type = "Unknown"
      break

    case "Link":
    case "SymbolicLink":
    case "CharacterDevice":
    case "BlockDevice":
    case "Directory":
    case "FIFO":
    default:
      type = tar.types[props.type]
  }

  this.type = type
  this.path = props.path
  this.size = props.size

  // size is special, since it signals when the file needs to end.
  this._remaining = props.size
}
```
- example usage
```shell
...
// a file parse operation.  Freeze it at its current state.
this._global = {}
var me = this
Object.keys(global || {}).forEach(function (g) {
  me._global[g] = global[g]
})

this._setProps()
}

inherits(Entry, Stream)

Entry.prototype.write = function (c) {
if (this._ending) this.error("write() after end()", null, true)
if (this._remaining === 0) {
...
```

#### <a name="apidoc.element.tar.entry.prototype.abort"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>abort ()](#apidoc.element.tar.entry.prototype.abort)
- description and source-code
```javascript
abort = function (){
  this._abort = true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry.prototype.end"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>end (c)](#apidoc.element.tar.entry.prototype.end)
- description and source-code
```javascript
end = function (c) {
  if (c) this.write(c)
  this._ending = true
  this._read()
}
```
- example usage
```shell
...

EntryWriter.prototype.add = function (entry) {
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
...
```

#### <a name="apidoc.element.tar.entry.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>pause ()](#apidoc.element.tar.entry.prototype.pause)
- description and source-code
```javascript
pause = function () {
  this._paused = true
  this.emit("pause")
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>resume ()](#apidoc.element.tar.entry.prototype.resume)
- description and source-code
```javascript
resume = function () {
  // console.error("    Tar Entry resume", this.path)
  this.emit("resume")
  this._paused = false
  this._read()
  return this._queueLen - this._index > 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry.prototype.write"></a>[function <span class="apidocSignatureSpan">tar.entry.prototype.</span>write (c)](#apidoc.element.tar.entry.prototype.write)
- description and source-code
```javascript
write = function (c) {
  if (this._ending) this.error("write() after end()", null, true)
  if (this._remaining === 0) {
    this.error("invalid bytes past eof")
  }

  // often we'll get a bunch of \0 at the end of the last write,
  // since chunks will always be 512 bytes when reading a tarball.
  if (c.length > this._remaining) {
    c = c.slice(0, this._remaining)
  }
  this._remaining -= c.length

  // put it on the stack.
  var ql = this._queueLen
  this._queue.push(c)
  this._queueLen ++

  this._read()

  // either paused, or buffered
  if (this._paused || ql > 0) {
    this._needDrain = true
    return false
  }

  return true
}
```
- example usage
```shell
...
  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
// console.error(".. .. .. i=%d", i)

var c = buf[i]

if (c === EOF) this._stream.end()
else this._stream.write(c)

if (this._paused) {
  // console.error(".. .. .. paused mid-emission")
  this._processing = false
  if (i < buf.length) {
    this._needDrain = true
    this._buffer = buf.slice(i + 1)
...
```



# <a name="apidoc.module.tar.entry_writer"></a>[module tar.entry_writer](#apidoc.module.tar.entry_writer)

#### <a name="apidoc.element.tar.entry_writer.entry_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>entry_writer (props)](#apidoc.element.tar.entry_writer.entry_writer)
- description and source-code
```javascript
function EntryWriter(props) {
  var me = this

  if (!(me instanceof EntryWriter)) {
    return new EntryWriter(props)
  }

  Stream.apply(this)

  me.writable = true
  me.readable = true

  me._stream = new BlockStream(512)

  me._stream.on("data", function (c) {
    me.emit("data", c)
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })

  me._stream.on("end", function () {
    me.emit("end")
    me.emit("close")
  })

  me.props = props
  if (props.type === "Directory") {
    props.size = 0
  }
  props.ustar = "ustar\0"
  props.ustarver = "00"
  me.path = props.path

  me._buffer = []
  me._didHeader = false
  me._meta = false

  me.on("pipe", function () {
    me._process()
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry_writer.super_"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.</span>super_ ()](#apidoc.element.tar.entry_writer.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.entry_writer.prototype"></a>[module tar.entry_writer.prototype](#apidoc.module.tar.entry_writer.prototype)

#### <a name="apidoc.element.tar.entry_writer.prototype._header"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>_header ()](#apidoc.element.tar.entry_writer.prototype._header)
- description and source-code
```javascript
_header = function () {
  // console.error(".. ew header")
  if (this._didHeader) return
  this._didHeader = true

  var headerBlock = TarHeader.encode(this.props)

  if (this.props.needExtended && !this._meta) {
    var me = this

    ExtendedHeaderWriter = ExtendedHeaderWriter ||
      require("./extended-header-writer.js")

    ExtendedHeaderWriter(this.props)
      .on("data", function (c) {
        me.emit("data", c)
      })
      .on("error", function (er) {
        me.emit("error", er)
      })
      .end()
  }

  // console.error(".. .. ew headerBlock emitting")
  this.emit("data", headerBlock)
  this.emit("header")
}
```
- example usage
```shell
...
this.emit("data", headerBlock)
this.emit("header")
}

EntryWriter.prototype._process = function () {
// console.error(".. .. ew process")
if (!this._didHeader && !this._meta) {
  this._header()
}

if (this._paused || this._processing) {
  // console.error(".. .. .. paused=%j, processing=%j", this._paused, this._processing)
  return
}
...
```

#### <a name="apidoc.element.tar.entry_writer.prototype._process"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>_process ()](#apidoc.element.tar.entry_writer.prototype._process)
- description and source-code
```javascript
_process = function () {
  // console.error(".. .. ew process")
  if (!this._didHeader && !this._meta) {
    this._header()
  }

  if (this._paused || this._processing) {
    // console.error(".. .. .. paused=%j, processing=%j", this._paused, this._processing)
    return
  }

  this._processing = true

  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
    // console.error(".. .. .. i=%d", i)

    var c = buf[i]

    if (c === EOF) this._stream.end()
    else this._stream.write(c)

    if (this._paused) {
      // console.error(".. .. .. paused mid-emission")
      this._processing = false
      if (i < buf.length) {
        this._needDrain = true
        this._buffer = buf.slice(i + 1)
      }
      return
    }
  }

  // console.error(".. .. .. emitted")
  this._buffer.length = 0
  this._processing = false

  // console.error(".. .. .. emitting drain")
  this.emit("drain")
}
```
- example usage
```shell
...
me.path = props.path

me._buffer = []
me._didHeader = false
me._meta = false

me.on("pipe", function () {
  me._process()
})
}

EntryWriter.prototype.write = function (c) {
// console.error(".. ew write")
if (this._ended) return this.emit("error", new Error("write after end"))
this._buffer.push(c)
...
```

#### <a name="apidoc.element.tar.entry_writer.prototype.add"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>add (entry)](#apidoc.element.tar.entry_writer.prototype.add)
- description and source-code
```javascript
add = function (entry) {
  // console.error(".. ew add")
  if (!this.parent) return this.emit("error", new Error("no parent"))

  // make sure that the _header and such is emitted, and clear out
  // the _currentEntry link on the parent.
  if (!this._ended) this.end()

  return this.parent.add(entry)
}
```
- example usage
```shell
...
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
this._didHeader = true
...
```

#### <a name="apidoc.element.tar.entry_writer.prototype.destroy"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>destroy ()](#apidoc.element.tar.entry_writer.prototype.destroy)
- description and source-code
```javascript
destroy = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry_writer.prototype.end"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>end (c)](#apidoc.element.tar.entry_writer.prototype.end)
- description and source-code
```javascript
end = function (c) {
  // console.error(".. ew end")
  if (c) this._buffer.push(c)
  this._buffer.push(EOF)
  this._ended = true
  this._process()
  this._needDrain = this._buffer.length > 0
}
```
- example usage
```shell
...

EntryWriter.prototype.add = function (entry) {
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
...
```

#### <a name="apidoc.element.tar.entry_writer.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>pause ()](#apidoc.element.tar.entry_writer.prototype.pause)
- description and source-code
```javascript
pause = function () {
  // console.error(".. ew pause")
  this._paused = true
  this.emit("pause")
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry_writer.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>resume ()](#apidoc.element.tar.entry_writer.prototype.resume)
- description and source-code
```javascript
resume = function () {
  // console.error(".. ew resume")
  this._paused = false
  this.emit("resume")
  this._process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.entry_writer.prototype.write"></a>[function <span class="apidocSignatureSpan">tar.entry_writer.prototype.</span>write (c)](#apidoc.element.tar.entry_writer.prototype.write)
- description and source-code
```javascript
write = function (c) {
  // console.error(".. ew write")
  if (this._ended) return this.emit("error", new Error("write after end"))
  this._buffer.push(c)
  this._process()
  this._needDrain = this._buffer.length > 0
  return !this._needDrain
}
```
- example usage
```shell
...
  var buf = this._buffer
  for (var i = 0; i < buf.length; i ++) {
// console.error(".. .. .. i=%d", i)

var c = buf[i]

if (c === EOF) this._stream.end()
else this._stream.write(c)

if (this._paused) {
  // console.error(".. .. .. paused mid-emission")
  this._processing = false
  if (i < buf.length) {
    this._needDrain = true
    this._buffer = buf.slice(i + 1)
...
```



# <a name="apidoc.module.tar.extended_header"></a>[module tar.extended_header](#apidoc.module.tar.extended_header)

#### <a name="apidoc.element.tar.extended_header.extended_header"></a>[function <span class="apidocSignatureSpan">tar.</span>extended_header ()](#apidoc.element.tar.extended_header.extended_header)
- description and source-code
```javascript
function ExtendedHeader() {
  Entry.apply(this, arguments)
  this.on("data", this._parse)
  this.fields = {}
  this._position = 0
  this._fieldPos = 0
  this._state = SIZE
  this._sizeBuf = []
  this._keyBuf = []
  this._valBuf = []
  this._size = -1
  this._key = ""
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.extended_header.super_"></a>[function <span class="apidocSignatureSpan">tar.extended_header.</span>super_ (header, extended, global)](#apidoc.element.tar.extended_header.super_)
- description and source-code
```javascript
function Entry(header, extended, global) {
  Stream.call(this)
  this.readable = true
  this.writable = true

  this._needDrain = false
  this._paused = false
  this._reading = false
  this._ending = false
  this._ended = false
  this._remaining = 0
  this._abort = false
  this._queue = []
  this._index = 0
  this._queueLen = 0

  this._read = this._read.bind(this)

  this.props = {}
  this._header = header
  this._extended = extended || {}

  // globals can change throughout the course of
  // a file parse operation.  Freeze it at its current state.
  this._global = {}
  var me = this
  Object.keys(global || {}).forEach(function (g) {
    me._global[g] = global[g]
  })

  this._setProps()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.extended_header.prototype"></a>[module tar.extended_header.prototype](#apidoc.module.tar.extended_header.prototype)

#### <a name="apidoc.element.tar.extended_header.prototype._parse"></a>[function <span class="apidocSignatureSpan">tar.extended_header.prototype.</span>_parse (c)](#apidoc.element.tar.extended_header.prototype._parse)
- description and source-code
```javascript
function parse(c) {
  if (this._state === ERR) return

  for ( var i = 0, l = c.length
      ; i < l
      ; this._position++, this._fieldPos++, i++) {
    // console.error("top of loop, size="+this._size)

    var b = c[i]

    if (this._size >= 0 && this._fieldPos > this._size) {
      error(this, "field exceeds length="+this._size)
      return
    }

    switch (this._state) {
      case ERR: return

      case SIZE:
        // console.error("parsing size, b=%d, rest=%j", b, c.slice(i).toString())
        if (b === space) {
          this._state = KEY
          // this._fieldPos = this._sizeBuf.length
          this._size = parseInt(new Buffer(this._sizeBuf).toString(), 10)
          this._sizeBuf.length = 0
          continue
        }
        if (b < _0 || b > _9) {
          error(this, "expected [" + _0 + ".." + _9 + "], got " + b)
          return
        }
        this._sizeBuf.push(b)
        continue

      case KEY:
        // can be any char except =, not > size.
        if (b === eq) {
          this._state = VAL
          this._key = new Buffer(this._keyBuf).toString()
          if (keyTrans[this._key]) this._key = keyTrans[this._key]
          this._keyBuf.length = 0
          continue
        }
        this._keyBuf.push(b)
        continue

      case VAL:
        // field must end with cr
        if (this._fieldPos === this._size - 1) {
          // console.error("finished with "+this._key)
          if (b !== cr) {
            error(this, "expected \\n at end of field")
            return
          }
          var val = new Buffer(this._valBuf).toString()
          if (numeric[this._key]) {
            val = parseFloat(val)
          }
          this.fields[this._key] = val

          this._valBuf.length = 0
          this._state = SIZE
          this._size = -1
          this._fieldPos = -1
          continue
        }
        this._valBuf.push(b)
        continue
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.extended_header_writer"></a>[module tar.extended_header_writer](#apidoc.module.tar.extended_header_writer)

#### <a name="apidoc.element.tar.extended_header_writer.extended_header_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>extended_header_writer (props)](#apidoc.element.tar.extended_header_writer.extended_header_writer)
- description and source-code
```javascript
function ExtendedHeaderWriter(props) {
  // console.error(">> ehw ctor")
  var me = this

  if (!(me instanceof ExtendedHeaderWriter)) {
    return new ExtendedHeaderWriter(props)
  }

  me.fields = props

  var p =
    { path : ("PaxHeader" + path.join("/", props.path || ""))
             .replace(/\\/g, "/").substr(0, 100)
    , mode : props.mode || 0666
    , uid : props.uid || 0
    , gid : props.gid || 0
    , size : 0 // will be set later
    , mtime : props.mtime || Date.now() / 1000
    , type : "x"
    , linkpath : ""
    , ustar : "ustar\0"
    , ustarver : "00"
    , uname : props.uname || ""
    , gname : props.gname || ""
    , devmaj : props.devmaj || 0
    , devmin : props.devmin || 0
    }


  EntryWriter.call(me, p)
  // console.error(">> ehw props", me.props)
  me.props = p

  me._meta = true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.extended_header_writer.super_"></a>[function <span class="apidocSignatureSpan">tar.extended_header_writer.</span>super_ (props)](#apidoc.element.tar.extended_header_writer.super_)
- description and source-code
```javascript
function EntryWriter(props) {
  var me = this

  if (!(me instanceof EntryWriter)) {
    return new EntryWriter(props)
  }

  Stream.apply(this)

  me.writable = true
  me.readable = true

  me._stream = new BlockStream(512)

  me._stream.on("data", function (c) {
    me.emit("data", c)
  })

  me._stream.on("drain", function () {
    me.emit("drain")
  })

  me._stream.on("end", function () {
    me.emit("end")
    me.emit("close")
  })

  me.props = props
  if (props.type === "Directory") {
    props.size = 0
  }
  props.ustar = "ustar\0"
  props.ustarver = "00"
  me.path = props.path

  me._buffer = []
  me._didHeader = false
  me._meta = false

  me.on("pipe", function () {
    me._process()
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.extended_header_writer.prototype"></a>[module tar.extended_header_writer.prototype](#apidoc.module.tar.extended_header_writer.prototype)

#### <a name="apidoc.element.tar.extended_header_writer.prototype._encodeFields"></a>[function <span class="apidocSignatureSpan">tar.extended_header_writer.prototype.</span>_encodeFields ()](#apidoc.element.tar.extended_header_writer.prototype._encodeFields)
- description and source-code
```javascript
_encodeFields = function () {
  // console.error(">> ehw _encodeFields")
  this.body = []
  if (this.fields.prefix) {
    this.fields.path = this.fields.prefix + "/" + this.fields.path
    this.fields.prefix = ""
  }
  encodeFields(this.fields, "", this.body, this.fields.noProprietary)
  var me = this
  this.body.forEach(function (l) {
    me.props.size += l.length
  })
}
```
- example usage
```shell
...
ExtendedHeaderWriter.prototype.end = function () {
// console.error(">> ehw end")
var me = this

if (me._ended) return
me._ended = true

me._encodeFields()

if (me.props.size === 0) {
  // nothing to write!
  me._ready = true
  me._stream.end()
  return
}
...
```

#### <a name="apidoc.element.tar.extended_header_writer.prototype.end"></a>[function <span class="apidocSignatureSpan">tar.extended_header_writer.prototype.</span>end ()](#apidoc.element.tar.extended_header_writer.prototype.end)
- description and source-code
```javascript
end = function () {
  // console.error(">> ehw end")
  var me = this

  if (me._ended) return
  me._ended = true

  me._encodeFields()

  if (me.props.size === 0) {
    // nothing to write!
    me._ready = true
    me._stream.end()
    return
  }

  me._stream.write(TarHeader.encode(me.props))
  me.body.forEach(function (l) {
    me._stream.write(l)
  })
  me._ready = true

  // console.error(">> ehw _process calling end()", me.props)
  this._stream.end()
}
```
- example usage
```shell
...

EntryWriter.prototype.add = function (entry) {
// console.error(".. ew add")
if (!this.parent) return this.emit("error", new Error("no parent"))

// make sure that the _header and such is emitted, and clear out
// the _currentEntry link on the parent.
if (!this._ended) this.end()

return this.parent.add(entry)
}

EntryWriter.prototype._header = function () {
// console.error(".. ew header")
if (this._didHeader) return
...
```



# <a name="apidoc.module.tar.global_header_writer"></a>[module tar.global_header_writer](#apidoc.module.tar.global_header_writer)

#### <a name="apidoc.element.tar.global_header_writer.global_header_writer"></a>[function <span class="apidocSignatureSpan">tar.</span>global_header_writer (props)](#apidoc.element.tar.global_header_writer.global_header_writer)
- description and source-code
```javascript
function GlobalHeaderWriter(props) {
  if (!(this instanceof GlobalHeaderWriter)) {
    return new GlobalHeaderWriter(props)
  }
  ExtendedHeaderWriter.call(this, props)
  this.props.type = "g"
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.global_header_writer.super_"></a>[function <span class="apidocSignatureSpan">tar.global_header_writer.</span>super_ (props)](#apidoc.element.tar.global_header_writer.super_)
- description and source-code
```javascript
function ExtendedHeaderWriter(props) {
  // console.error(">> ehw ctor")
  var me = this

  if (!(me instanceof ExtendedHeaderWriter)) {
    return new ExtendedHeaderWriter(props)
  }

  me.fields = props

  var p =
    { path : ("PaxHeader" + path.join("/", props.path || ""))
             .replace(/\\/g, "/").substr(0, 100)
    , mode : props.mode || 0666
    , uid : props.uid || 0
    , gid : props.gid || 0
    , size : 0 // will be set later
    , mtime : props.mtime || Date.now() / 1000
    , type : "x"
    , linkpath : ""
    , ustar : "ustar\0"
    , ustarver : "00"
    , uname : props.uname || ""
    , gname : props.gname || ""
    , devmaj : props.devmaj || 0
    , devmin : props.devmin || 0
    }


  EntryWriter.call(me, p)
  // console.error(">> ehw props", me.props)
  me.props = p

  me._meta = true
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.header"></a>[module tar.header](#apidoc.module.tar.header)

#### <a name="apidoc.element.tar.header.header"></a>[function <span class="apidocSignatureSpan">tar.</span>header (block)](#apidoc.element.tar.header.header)
- description and source-code
```javascript
function TarHeader(block) {
  if (!(this instanceof TarHeader)) return new TarHeader(block)
  if (block) this.decode(block)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.header.decode"></a>[function <span class="apidocSignatureSpan">tar.header.</span>decode (block)](#apidoc.element.tar.header.decode)
- description and source-code
```javascript
function decode(block) {
  block = block || this.block
  assert(Buffer.isBuffer(block) && block.length === 512)

  this.block = block
  this.cksumValid = this.checkSum()

  var prefix = null

  // slice off each field.
  for (var f = 0; fields[f] !== null; f ++) {
    var field = fields[f]
      , val = block.slice(fieldOffs[f], fieldEnds[f])

    switch (field) {
      case "ustar":
        // if not ustar, then everything after that is just padding.
        if (val.toString() !== "ustar\0") {
          this.ustar = false
          return
        } else {
          // console.error("ustar:", val, val.toString())
          this.ustar = val.toString()
        }
        break

      // prefix is special, since it might signal the xstar header
      case "prefix":
        var atime = parseNumeric(val.slice(131, 131 + 12))
          , ctime = parseNumeric(val.slice(131 + 12, 131 + 12 + 12))
        if ((val[130] === 0 || val[130] === space) &&
            typeof atime === "number" &&
            typeof ctime === "number" &&
            val[131 + 12] === space &&
            val[131 + 12 + 12] === space) {
          this.atime = atime
          this.ctime = ctime
          val = val.slice(0, 130)
        }
        prefix = val.toString("utf8").replace(/\0+$/, "")
        // console.error("%% header reading prefix", prefix)
        break

      // all other fields are null-padding text
      // or a number.
      default:
        if (numeric[field]) {
          this[field] = parseNumeric(val)
        } else {
          this[field] = val.toString("utf8").replace(/\0+$/, "")
        }
        break
    }
  }

  // if we got a prefix, then prepend it to the path.
  if (prefix) {
    this.path = prefix + "/" + this.path
    // console.error("%% header got a prefix", this.path)
  }
}
```
- example usage
```shell
...
, assert = require("assert").ok
, space = " ".charCodeAt(0)
, slash = "/".charCodeAt(0)
, bslash = process.platform === "win32" ? "\\".charCodeAt(0) : null

function TarHeader (block) {
if (!(this instanceof TarHeader)) return new TarHeader(block)
if (block) this.decode(block)
}

TarHeader.prototype =
{ decode : decode
, encode: encode
, calcSum: calcSum
, checkSum: checkSum
...
```

#### <a name="apidoc.element.tar.header.encode"></a>[function <span class="apidocSignatureSpan">tar.header.</span>encode (obj)](#apidoc.element.tar.header.encode)
- description and source-code
```javascript
function encode(obj) {
  if (!obj && !(this instanceof TarHeader)) throw new Error(
    "encode must be called on a TarHeader, or supplied an object")

  obj = obj || this
  var block = obj.block = new Buffer(512)

  // if the object has a "prefix", then that's actually an extension of
  // the path field.
  if (obj.prefix) {
    // console.error("%% header encoding, got a prefix", obj.prefix)
    obj.path = obj.prefix + "/" + obj.path
    // console.error("%% header encoding, prefixed path", obj.path)
    obj.prefix = ""
  }

  obj.needExtended = false

  if (obj.mode) {
    if (typeof obj.mode === "string") obj.mode = parseInt(obj.mode, 8)
    obj.mode = obj.mode & 0777
  }

  for (var f = 0; fields[f] !== null; f ++) {
    var field = fields[f]
      , off = fieldOffs[f]
      , end = fieldEnds[f]
      , ret

    switch (field) {
      case "cksum":
        // special, done below, after all the others
        break

      case "prefix":
        // special, this is an extension of the "path" field.
        // console.error("%% header encoding, skip prefix later")
        break

      case "type":
        // convert from long name to a single char.
        var type = obj.type || "0"
        if (type.length > 1) {
          type = tar.types[obj.type]
          if (!type) type = "0"
        }
        writeText(block, off, end, type)
        break

      case "path":
        // uses the "prefix" field if > 100 bytes, but <= 255
        var pathLen = Buffer.byteLength(obj.path)
          , pathFSize = fieldSize[fields.path]
          , prefFSize = fieldSize[fields.prefix]

        // paths between 100 and 255 should use the prefix field.
        // longer than 255
        if (pathLen > pathFSize &&
            pathLen <= pathFSize + prefFSize) {
          // need to find a slash somewhere in the middle so that
          // path and prefix both fit in their respective fields
          var searchStart = pathLen - 1 - pathFSize
            , searchEnd = prefFSize
            , found = false
            , pathBuf = new Buffer(obj.path)

          for ( var s = searchStart
              ; (s <= searchEnd)
              ; s ++ ) {
            if (pathBuf[s] === slash || pathBuf[s] === bslash) {
              found = s
              break
            }
          }

          if (found !== false) {
            prefix = pathBuf.slice(0, found).toString("utf8")
            path = pathBuf.slice(found + 1).toString("utf8")

            ret = writeText(block, off, end, path)
            off = fieldOffs[fields.prefix]
            end = fieldEnds[fields.prefix]
            // console.error("%% header writing prefix", off, end, prefix)
            ret = writeText(block, off, end, prefix) || ret
            break
          }
        }

        // paths less than 100 chars don't need a prefix
        // and paths longer than 255 need an extended header and will fail
        // on old implementations no matter what we do here.
        // Null out the prefix, and fallthrough to default.
        // console.error("%% header writing no prefix")
        var poff = fieldOffs[fields.prefix]
          , pend = fieldEnds[fields.prefix]
        writeText(block, poff, pend, "")
        // fallthrough

      // all other fields are numeric or text
      default:
        ret = numeric[field]
            ? writeNumeric(block, off, end, obj[field])
            : writeText(block, off, end, obj[field] || "")
        break
    }
    obj.needExtended = obj.needExtended || ret
  }

  var off = fieldOffs[fields.cksum]
    , end = fieldEnds[fields.cksum]

  writeNumeric(block, off, end, calcSum.call(this, block))

  return block
}
```
- example usage
```shell
...
}

EntryWriter.prototype._header = function () {
  // console.error(".. ew header")
  if (this._didHeader) return
  this._didHeader = true

  var headerBlock = TarHeader.encode(this.props)

  if (this.props.needExtended && !this._meta) {
var me = this

ExtendedHeaderWriter = ExtendedHeaderWriter ||
  require("./extended-header-writer.js")
...
```

#### <a name="apidoc.element.tar.header.parseNumeric"></a>[function <span class="apidocSignatureSpan">tar.header.</span>parseNumeric (f)](#apidoc.element.tar.header.parseNumeric)
- description and source-code
```javascript
function parseNumeric(f) {
  if (f[0] & 0x80) return parse256(f)

  var str = f.toString("utf8").split("\0")[0].trim()
    , res = parseInt(str, 8)

  return isNaN(res) ? null : res
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar.header.prototype"></a>[module tar.header.prototype](#apidoc.module.tar.header.prototype)

#### <a name="apidoc.element.tar.header.prototype.calcSum"></a>[function <span class="apidocSignatureSpan">tar.header.prototype.</span>calcSum (block)](#apidoc.element.tar.header.prototype.calcSum)
- description and source-code
```javascript
function calcSum(block) {
  block = block || this.block
  assert(Buffer.isBuffer(block) && block.length === 512)

  if (!block) throw new Error("Need block to checksum")

  // now figure out what it would be if the cksum was "        "
  var sum = 0
    , start = fieldOffs[fields.cksum]
    , end = fieldEnds[fields.cksum]

  for (var i = 0; i < fieldOffs[fields.cksum]; i ++) {
    sum += block[i]
  }

  for (var i = start; i < end; i ++) {
    sum += space
  }

  for (var i = end; i < 512; i ++) {
    sum += block[i]
  }

  return sum
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar.header.prototype.checkSum"></a>[function <span class="apidocSignatureSpan">tar.header.prototype.</span>checkSum (block)](#apidoc.element.tar.header.prototype.checkSum)
- description and source-code
```javascript
function checkSum(block) {
  var sum = calcSum.call(this, block)
  block = block || this.block

  var cksum = block.slice(fieldOffs[fields.cksum], fieldEnds[fields.cksum])
  cksum = parseNumeric(cksum)

  return cksum === sum
}
```
- example usage
```shell
...
}

function decode (block) {
block = block || this.block
assert(Buffer.isBuffer(block) && block.length === 512)

this.block = block
this.cksumValid = this.checkSum()

var prefix = null

// slice off each field.
for (var f = 0; fields[f] !== null; f ++) {
  var field = fields[f]
    , val = block.slice(fieldOffs[f], fieldEnds[f])
...
```

#### <a name="apidoc.element.tar.header.prototype.decode"></a>[function <span class="apidocSignatureSpan">tar.header.prototype.</span>decode (block)](#apidoc.element.tar.header.prototype.decode)
- description and source-code
```javascript
function decode(block) {
  block = block || this.block
  assert(Buffer.isBuffer(block) && block.length === 512)

  this.block = block
  this.cksumValid = this.checkSum()

  var prefix = null

  // slice off each field.
  for (var f = 0; fields[f] !== null; f ++) {
    var field = fields[f]
      , val = block.slice(fieldOffs[f], fieldEnds[f])

    switch (field) {
      case "ustar":
        // if not ustar, then everything after that is just padding.
        if (val.toString() !== "ustar\0") {
          this.ustar = false
          return
        } else {
          // console.error("ustar:", val, val.toString())
          this.ustar = val.toString()
        }
        break

      // prefix is special, since it might signal the xstar header
      case "prefix":
        var atime = parseNumeric(val.slice(131, 131 + 12))
          , ctime = parseNumeric(val.slice(131 + 12, 131 + 12 + 12))
        if ((val[130] === 0 || val[130] === space) &&
            typeof atime === "number" &&
            typeof ctime === "number" &&
            val[131 + 12] === space &&
            val[131 + 12 + 12] === space) {
          this.atime = atime
          this.ctime = ctime
          val = val.slice(0, 130)
        }
        prefix = val.toString("utf8").replace(/\0+$/, "")
        // console.error("%% header reading prefix", prefix)
        break

      // all other fields are null-padding text
      // or a number.
      default:
        if (numeric[field]) {
          this[field] = parseNumeric(val)
        } else {
          this[field] = val.toString("utf8").replace(/\0+$/, "")
        }
        break
    }
  }

  // if we got a prefix, then prepend it to the path.
  if (prefix) {
    this.path = prefix + "/" + this.path
    // console.error("%% header got a prefix", this.path)
  }
}
```
- example usage
```shell
...
, assert = require("assert").ok
, space = " ".charCodeAt(0)
, slash = "/".charCodeAt(0)
, bslash = process.platform === "win32" ? "\\".charCodeAt(0) : null

function TarHeader (block) {
if (!(this instanceof TarHeader)) return new TarHeader(block)
if (block) this.decode(block)
}

TarHeader.prototype =
{ decode : decode
, encode: encode
, calcSum: calcSum
, checkSum: checkSum
...
```

#### <a name="apidoc.element.tar.header.prototype.encode"></a>[function <span class="apidocSignatureSpan">tar.header.prototype.</span>encode (obj)](#apidoc.element.tar.header.prototype.encode)
- description and source-code
```javascript
function encode(obj) {
  if (!obj && !(this instanceof TarHeader)) throw new Error(
    "encode must be called on a TarHeader, or supplied an object")

  obj = obj || this
  var block = obj.block = new Buffer(512)

  // if the object has a "prefix", then that's actually an extension of
  // the path field.
  if (obj.prefix) {
    // console.error("%% header encoding, got a prefix", obj.prefix)
    obj.path = obj.prefix + "/" + obj.path
    // console.error("%% header encoding, prefixed path", obj.path)
    obj.prefix = ""
  }

  obj.needExtended = false

  if (obj.mode) {
    if (typeof obj.mode === "string") obj.mode = parseInt(obj.mode, 8)
    obj.mode = obj.mode & 0777
  }

  for (var f = 0; fields[f] !== null; f ++) {
    var field = fields[f]
      , off = fieldOffs[f]
      , end = fieldEnds[f]
      , ret

    switch (field) {
      case "cksum":
        // special, done below, after all the others
        break

      case "prefix":
        // special, this is an extension of the "path" field.
        // console.error("%% header encoding, skip prefix later")
        break

      case "type":
        // convert from long name to a single char.
        var type = obj.type || "0"
        if (type.length > 1) {
          type = tar.types[obj.type]
          if (!type) type = "0"
        }
        writeText(block, off, end, type)
        break

      case "path":
        // uses the "prefix" field if > 100 bytes, but <= 255
        var pathLen = Buffer.byteLength(obj.path)
          , pathFSize = fieldSize[fields.path]
          , prefFSize = fieldSize[fields.prefix]

        // paths between 100 and 255 should use the prefix field.
        // longer than 255
        if (pathLen > pathFSize &&
            pathLen <= pathFSize + prefFSize) {
          // need to find a slash somewhere in the middle so that
          // path and prefix both fit in their respective fields
          var searchStart = pathLen - 1 - pathFSize
            , searchEnd = prefFSize
            , found = false
            , pathBuf = new Buffer(obj.path)

          for ( var s = searchStart
              ; (s <= searchEnd)
              ; s ++ ) {
            if (pathBuf[s] === slash || pathBuf[s] === bslash) {
              found = s
              break
            }
          }

          if (found !== false) {
            prefix = pathBuf.slice(0, found).toString("utf8")
            path = pathBuf.slice(found + 1).toString("utf8")

            ret = writeText(block, off, end, path)
            off = fieldOffs[fields.prefix]
            end = fieldEnds[fields.prefix]
            // console.error("%% header writing prefix", off, end, prefix)
            ret = writeText(block, off, end, prefix) || ret
            break
          }
        }

        // paths less than 100 chars don't need a prefix
        // and paths longer than 255 need an extended header and will fail
        // on old implementations no matter what we do here.
        // Null out the prefix, and fallthrough to default.
        // console.error("%% header writing no prefix")
        var poff = fieldOffs[fields.prefix]
          , pend = fieldEnds[fields.prefix]
        writeText(block, poff, pend, "")
        // fallthrough

      // all other fields are numeric or text
      default:
        ret = numeric[field]
            ? writeNumeric(block, off, end, obj[field])
            : writeText(block, off, end, obj[field] || "")
        break
    }
    obj.needExtended = obj.needExtended || ret
  }

  var off = fieldOffs[fields.cksum]
    , end = fieldEnds[fields.cksum]

  writeNumeric(block, off, end, calcSum.call(this, block))

  return block
}
```
- example usage
```shell
...
}

EntryWriter.prototype._header = function () {
  // console.error(".. ew header")
  if (this._didHeader) return
  this._didHeader = true

  var headerBlock = TarHeader.encode(this.props)

  if (this.props.needExtended && !this._meta) {
var me = this

ExtendedHeaderWriter = ExtendedHeaderWriter ||
  require("./extended-header-writer.js")
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
