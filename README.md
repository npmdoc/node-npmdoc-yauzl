# api documentation for  [yauzl (v2.7.0)](https://github.com/thejoshwolfe/yauzl)  [![npm package](https://img.shields.io/npm/v/npmdoc-yauzl.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-yauzl) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-yauzl.svg)](https://travis-ci.org/npmdoc/node-npmdoc-yauzl)
#### yet another unzip library for node

[![NPM](https://nodei.co/npm/yauzl.png?downloads=true)](https://www.npmjs.com/package/yauzl)

[![apidoc](https://npmdoc.github.io/node-npmdoc-yauzl/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-yauzl_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-yauzl/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-yauzl/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-yauzl/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Josh Wolfe",
        "email": "thejoshwolfe@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/thejoshwolfe/yauzl/issues"
    },
    "dependencies": {
        "buffer-crc32": "~0.2.3",
        "fd-slicer": "~1.0.1"
    },
    "description": "yet another unzip library for node",
    "devDependencies": {
        "bl": "~1.0.0",
        "istanbul": "~0.3.4",
        "pend": "~1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "e21d847868b496fc29eaec23ee87fdd33e9b2bce",
        "tarball": "https://registry.npmjs.org/yauzl/-/yauzl-2.7.0.tgz"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "1f5cb3dc6f4e9d4df06e96c665af52e576616cc3",
    "homepage": "https://github.com/thejoshwolfe/yauzl",
    "keywords": [
        "unzip",
        "zip",
        "stream",
        "archive",
        "file"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "thejoshwolfe",
            "email": "thejoshwolfe@gmail.com"
        },
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        }
    ],
    "name": "yauzl",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/thejoshwolfe/yauzl.git"
    },
    "scripts": {
        "test": "node test/test.js",
        "test-cov": "istanbul cover test/test.js",
        "test-travis": "istanbul cover --report lcovonly test/test.js"
    },
    "version": "2.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module yauzl](#apidoc.module.yauzl)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>Entry ()](#apidoc.element.yauzl.Entry)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>RandomAccessReader ()](#apidoc.element.yauzl.RandomAccessReader)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>ZipFile (reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings)](#apidoc.element.yauzl.ZipFile)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>dosDateTimeToDate (date, time)](#apidoc.element.yauzl.dosDateTimeToDate)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>fromBuffer (buffer, options, callback)](#apidoc.element.yauzl.fromBuffer)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>fromFd (fd, options, callback)](#apidoc.element.yauzl.fromFd)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>fromRandomAccessReader (reader, totalSize, options, callback)](#apidoc.element.yauzl.fromRandomAccessReader)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>open (path, options, callback)](#apidoc.element.yauzl.open)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>validateFileName (fileName)](#apidoc.element.yauzl.validateFileName)
1.  object <span class="apidocSignatureSpan">yauzl.</span>Entry.prototype
1.  object <span class="apidocSignatureSpan">yauzl.</span>RandomAccessReader.prototype
1.  object <span class="apidocSignatureSpan">yauzl.</span>ZipFile.prototype

#### [module yauzl.Entry](#apidoc.module.yauzl.Entry)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>Entry ()](#apidoc.element.yauzl.Entry.Entry)

#### [module yauzl.Entry.prototype](#apidoc.module.yauzl.Entry.prototype)
1.  [function <span class="apidocSignatureSpan">yauzl.Entry.prototype.</span>getLastModDate ()](#apidoc.element.yauzl.Entry.prototype.getLastModDate)

#### [module yauzl.RandomAccessReader](#apidoc.module.yauzl.RandomAccessReader)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>RandomAccessReader ()](#apidoc.element.yauzl.RandomAccessReader.RandomAccessReader)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.</span>super_ ()](#apidoc.element.yauzl.RandomAccessReader.super_)

#### [module yauzl.RandomAccessReader.prototype](#apidoc.module.yauzl.RandomAccessReader.prototype)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>_readStreamForRange (start, end)](#apidoc.element.yauzl.RandomAccessReader.prototype._readStreamForRange)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>close (callback)](#apidoc.element.yauzl.RandomAccessReader.prototype.close)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>createReadStream (options)](#apidoc.element.yauzl.RandomAccessReader.prototype.createReadStream)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>read (buffer, offset, length, position, callback)](#apidoc.element.yauzl.RandomAccessReader.prototype.read)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>ref ()](#apidoc.element.yauzl.RandomAccessReader.prototype.ref)
1.  [function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>unref ()](#apidoc.element.yauzl.RandomAccessReader.prototype.unref)

#### [module yauzl.ZipFile](#apidoc.module.yauzl.ZipFile)
1.  [function <span class="apidocSignatureSpan">yauzl.</span>ZipFile (reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings)](#apidoc.element.yauzl.ZipFile.ZipFile)
1.  [function <span class="apidocSignatureSpan">yauzl.ZipFile.</span>super_ ()](#apidoc.element.yauzl.ZipFile.super_)

#### [module yauzl.ZipFile.prototype](#apidoc.module.yauzl.ZipFile.prototype)
1.  [function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>close ()](#apidoc.element.yauzl.ZipFile.prototype.close)
1.  [function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>openReadStream (entry, callback)](#apidoc.element.yauzl.ZipFile.prototype.openReadStream)
1.  [function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>readEntry ()](#apidoc.element.yauzl.ZipFile.prototype.readEntry)



# <a name="apidoc.module.yauzl"></a>[module yauzl](#apidoc.module.yauzl)

#### <a name="apidoc.element.yauzl.Entry"></a>[function <span class="apidocSignatureSpan">yauzl.</span>Entry ()](#apidoc.element.yauzl.Entry)
- description and source-code
```javascript
function Entry() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.RandomAccessReader"></a>[function <span class="apidocSignatureSpan">yauzl.</span>RandomAccessReader ()](#apidoc.element.yauzl.RandomAccessReader)
- description and source-code
```javascript
function RandomAccessReader() {
  EventEmitter.call(this);
  this.refCount = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.ZipFile"></a>[function <span class="apidocSignatureSpan">yauzl.</span>ZipFile (reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings)](#apidoc.element.yauzl.ZipFile)
- description and source-code
```javascript
function ZipFile(reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings) {
  var self = this;
  EventEmitter.call(self);
  self.reader = reader;
  // forward close events
  self.reader.on("error", function(err) {
    // error closing the fd
    emitError(self, err);
  });
  self.reader.once("close", function() {
    self.emit("close");
  });
  self.readEntryCursor = centralDirectoryOffset;
  self.fileSize = fileSize;
  self.entryCount = entryCount;
  self.comment = comment;
  self.entriesRead = 0;
  self.autoClose = !!autoClose;
  self.lazyEntries = !!lazyEntries;
  self.decodeStrings = !!decodeStrings;
  self.isOpen = true;
  self.emittedError = false;

  if (!self.lazyEntries) self.readEntry();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.dosDateTimeToDate"></a>[function <span class="apidocSignatureSpan">yauzl.</span>dosDateTimeToDate (date, time)](#apidoc.element.yauzl.dosDateTimeToDate)
- description and source-code
```javascript
function dosDateTimeToDate(date, time) {
  var day = date & 0x1f; // 1-31
  var month = (date >> 5 & 0xf) - 1; // 1-12, 0-11
  var year = (date >> 9 & 0x7f) + 1980; // 0-128, 1980-2108

  var millisecond = 0;
  var second = (time & 0x1f) * 2; // 0-29, 0-58 (even numbers)
  var minute = time >> 5 & 0x3f; // 0-59
  var hour = time >> 11 & 0x1f; // 0-23

  return new Date(year, month, day, hour, minute, second, millisecond);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.fromBuffer"></a>[function <span class="apidocSignatureSpan">yauzl.</span>fromBuffer (buffer, options, callback)](#apidoc.element.yauzl.fromBuffer)
- description and source-code
```javascript
function fromBuffer(buffer, options, callback) {
  if (typeof options === "function") {
    callback = options;
    options = null;
  }
  if (options == null) options = {};
  options.autoClose = false;
  if (options.lazyEntries == null) options.lazyEntries = false;
  if (options.decodeStrings == null) options.decodeStrings = true;
  // i got your open file right here.
  var reader = fd_slicer.createFromBuffer(buffer);
  fromRandomAccessReader(reader, buffer.length, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.fromFd"></a>[function <span class="apidocSignatureSpan">yauzl.</span>fromFd (fd, options, callback)](#apidoc.element.yauzl.fromFd)
- description and source-code
```javascript
function fromFd(fd, options, callback) {
  if (typeof options === "function") {
    callback = options;
    options = null;
  }
  if (options == null) options = {};
  if (options.autoClose == null) options.autoClose = false;
  if (options.lazyEntries == null) options.lazyEntries = false;
  if (options.decodeStrings == null) options.decodeStrings = true;
  if (callback == null) callback = defaultCallback;
  fs.fstat(fd, function(err, stats) {
    if (err) return callback(err);
    var reader = fd_slicer.createFromFd(fd, {autoClose: true});
    fromRandomAccessReader(reader, stats.size, options, callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.fromRandomAccessReader"></a>[function <span class="apidocSignatureSpan">yauzl.</span>fromRandomAccessReader (reader, totalSize, options, callback)](#apidoc.element.yauzl.fromRandomAccessReader)
- description and source-code
```javascript
function fromRandomAccessReader(reader, totalSize, options, callback) {
  if (typeof options === "function") {
    callback = options;
    options = null;
  }
  if (options == null) options = {};
  if (options.autoClose == null) options.autoClose = true;
  if (options.lazyEntries == null) options.lazyEntries = false;
  if (options.decodeStrings == null) options.decodeStrings = true;
  var decodeStrings = !!options.decodeStrings;
  if (callback == null) callback = defaultCallback;
  if (typeof totalSize !== "number") throw new Error("expected totalSize parameter to be a number");
  if (totalSize > Number.MAX_SAFE_INTEGER) {
    throw new Error("zip file too large. only file sizes up to 2^52 are supported due to JavaScript's Number type being an IEEE
754 double.");
  }

  // the matching unref() call is in zipfile.close()
  reader.ref();

  // eocdr means End of Central Directory Record.
  // search backwards for the eocdr signature.
  // the last field of the eocdr is a variable-length comment.
  // the comment size is encoded in a 2-byte field in the eocdr, which we can't find without trudging backwards through the comment
 to find it.
  // as a consequence of this design decision, it's possible to have ambiguous zip file metadata if a coherent eocdr was in the
comment.
  // we search backwards for a eocdr signature, and hope that whoever made the zip file was smart enough to forbid the eocdr signature
 in the comment.
  var eocdrWithoutCommentSize = 22;
  var maxCommentSize = 0x10000; // 2-byte size
  var bufferSize = Math.min(eocdrWithoutCommentSize + maxCommentSize, totalSize);
  var buffer = new Buffer(bufferSize);
  var bufferReadStart = totalSize - buffer.length;
  readAndAssertNoEof(reader, buffer, 0, bufferSize, bufferReadStart, function(err) {
    if (err) return callback(err);
    for (var i = bufferSize - eocdrWithoutCommentSize; i >= 0; i -= 1) {
      if (buffer.readUInt32LE(i) !== 0x06054b50) continue;
      // found eocdr
      var eocdrBuffer = buffer.slice(i);

      // 0 - End of central directory signature = 0x06054b50
      // 4 - Number of this disk
      var diskNumber = eocdrBuffer.readUInt16LE(4);
      if (diskNumber !== 0) {
        return callback(new Error("multi-disk zip files are not supported: found disk number: " + diskNumber));
      }
      // 6 - Disk where central directory starts
      // 8 - Number of central directory records on this disk
      // 10 - Total number of central directory records
      var entryCount = eocdrBuffer.readUInt16LE(10);
      // 12 - Size of central directory (bytes)
      // 16 - Offset of start of central directory, relative to start of archive
      var centralDirectoryOffset = eocdrBuffer.readUInt32LE(16);
      // 20 - Comment length
      var commentLength = eocdrBuffer.readUInt16LE(20);
      var expectedCommentLength = eocdrBuffer.length - eocdrWithoutCommentSize;
      if (commentLength !== expectedCommentLength) {
        return callback(new Error("invalid comment length. expected: " + expectedCommentLength + ". found: " + commentLength));
      }
      // 22 - Comment
      // the encoding is always cp437.
      var comment = decodeStrings ? decodeBuffer(eocdrBuffer, 22, eocdrBuffer.length, false)
                                  : eocdrBuffer.slice(22);

      if (!(entryCount === 0xffff || centralDirectoryOffset === 0xffffffff)) {
        return callback(null, new ZipFile(reader, centralDirectoryOffset, totalSize, entryCount, comment, options.autoClose, options
.lazyEntries, decodeStrings));
      }

      // ZIP64 format

      // ZIP64 Zip64 end of central directory locator
      var zip64EocdlBuffer = new Buffer(20);
      var zip64EocdlOffset = bufferReadStart + i - zip64EocdlBuffer.length;
      readAndAssertNoEof(reader, zip64EocdlBuffer, 0, zip64EocdlBuffer.length, zip64EocdlOffset, function(err) {
        if (err) return callback(err);

        // 0 - zip64 end of central dir locator signature = 0x07064b50
        if (zip64EocdlBuffer.readUInt32LE(0) !== 0x07064b50) {
          return callback(new Error("invalid zip64 end of central ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.open"></a>[function <span class="apidocSignatureSpan">yauzl.</span>open (path, options, callback)](#apidoc.element.yauzl.open)
- description and source-code
```javascript
function open(path, options, callback) {
  if (typeof options === "function") {
    callback = options;
    options = null;
  }
  if (options == null) options = {};
  if (options.autoClose == null) options.autoClose = true;
  if (options.lazyEntries == null) options.lazyEntries = false;
  if (options.decodeStrings == null) options.decodeStrings = true;
  if (callback == null) callback = defaultCallback;
  fs.open(path, "r", function(err, fd) {
    if (err) return callback(err);
    fromFd(fd, options, function(err, zipfile) {
      if (err) fs.close(fd, defaultCallback);
      callback(err, zipfile);
    });
  });
}
```
- example usage
```shell
...

'''js
var yauzl = require("yauzl");
var fs = require("fs");
var path = require("path");
var mkdirp = require("mkdirp"); // or similar

yauzl.open("path/to/file.zip", {lazyEntries: true}, function(err, zipfile) {
if (err) throw err;
zipfile.readEntry();
zipfile.on("entry", function(entry) {
  if (/\/$/.test(entry.fileName)) {
    // directory file names end with '/'
    mkdirp(entry.fileName, function(err) {
      if (err) throw err;
...
```

#### <a name="apidoc.element.yauzl.validateFileName"></a>[function <span class="apidocSignatureSpan">yauzl.</span>validateFileName (fileName)](#apidoc.element.yauzl.validateFileName)
- description and source-code
```javascript
function validateFileName(fileName) {
  if (fileName.indexOf("\\") !== -1) {
    return "invalid characters in fileName: " + fileName;
  }
  if (/^[a-zA-Z]:/.test(fileName) || /^\//.test(fileName)) {
    return "absolute path: " + fileName;
  }
  if (fileName.split("/").indexOf("..") !== -1) {
    return "invalid relative path: " + fileName;
  }
  // all good
  return null;
}
```
- example usage
```shell
...
### validateFileName(fileName)

Returns 'null' or a 'String' error message depending on the validity of 'fileName'.
If 'fileName' starts with '"/"' or '/[A-Za-z]:\//' or if it contains '".."' path segments or '"\\"',
this function returns an error message appropriate for use like this:

'''js
var errorMessage = yauzl.validateFileName(fileName);
if (errorMessage != null) throw new Error(errorMessage);
'''

This function is automatically run for each entry, as long as 'decodeStrings' is 'true'.
See 'open()' and 'Event: "entry"' for more information.

### Class: ZipFile
...
```



# <a name="apidoc.module.yauzl.Entry"></a>[module yauzl.Entry](#apidoc.module.yauzl.Entry)

#### <a name="apidoc.element.yauzl.Entry.Entry"></a>[function <span class="apidocSignatureSpan">yauzl.</span>Entry ()](#apidoc.element.yauzl.Entry.Entry)
- description and source-code
```javascript
function Entry() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yauzl.Entry.prototype"></a>[module yauzl.Entry.prototype](#apidoc.module.yauzl.Entry.prototype)

#### <a name="apidoc.element.yauzl.Entry.prototype.getLastModDate"></a>[function <span class="apidocSignatureSpan">yauzl.Entry.prototype.</span>getLastModDate ()](#apidoc.element.yauzl.Entry.prototype.getLastModDate)
- description and source-code
```javascript
getLastModDate = function () {
  return dosDateTimeToDate(this.lastModFileDate, this.lastModFileTime);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yauzl.RandomAccessReader"></a>[module yauzl.RandomAccessReader](#apidoc.module.yauzl.RandomAccessReader)

#### <a name="apidoc.element.yauzl.RandomAccessReader.RandomAccessReader"></a>[function <span class="apidocSignatureSpan">yauzl.</span>RandomAccessReader ()](#apidoc.element.yauzl.RandomAccessReader.RandomAccessReader)
- description and source-code
```javascript
function RandomAccessReader() {
  EventEmitter.call(this);
  this.refCount = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.super_"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.</span>super_ ()](#apidoc.element.yauzl.RandomAccessReader.super_)
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



# <a name="apidoc.module.yauzl.RandomAccessReader.prototype"></a>[module yauzl.RandomAccessReader.prototype](#apidoc.module.yauzl.RandomAccessReader.prototype)

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype._readStreamForRange"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>_readStreamForRange (start, end)](#apidoc.element.yauzl.RandomAccessReader.prototype._readStreamForRange)
- description and source-code
```javascript
_readStreamForRange = function (start, end) {
  throw new Error("not implemented");
}
```
- example usage
```shell
...
Such heuristics are outside the scope of this library,
but enforcing the 'uncompressedSize' is implemented here as a security feature.

It is possible to destroy the 'readStream' before it has piped all of its data.
To do this, call 'readStream.destroy()'.
You must 'unpipe()' the 'readStream' from any destination before calling 'readStream.destroy()'.
If this zipfile was created using 'fromRandomAccessReader()', the 'RandomAccessReader' implementation
must provide readable streams that implement a '.destroy()' method (see 'randomAccessReader._readStreamForRange()')
in order for calls to 'readStream.destroy()' to work in this context.

#### close()

Causes all future calls to 'openReadStream()' to fail,
and closes the fd after all streams created by 'openReadStream()' have emitted their 'end' events.
...
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype.close"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>close (callback)](#apidoc.element.yauzl.RandomAccessReader.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  setImmediate(callback);
}
```
- example usage
```shell
...

'options' may be omitted or 'null'. The defaults are '{autoClose: true, lazyEntries: false, decodeStrings: true}'.

'autoClose' is effectively equivalent to:

'''js
zipfile.once("end", function() {
  zipfile.close();
});
'''

'lazyEntries' indicates that entries should be read only when 'readEntry()' is called.
If 'lazyEntries' is 'false', 'entry' events will be emitted as fast as possible to allow 'pipe()'ing
file data from all entries in parallel.
This is not recommended, as it can lead to out of control memory usage for zip files with many entries.
...
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype.createReadStream"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>createReadStream (options)](#apidoc.element.yauzl.RandomAccessReader.prototype.createReadStream)
- description and source-code
```javascript
createReadStream = function (options) {
  var start = options.start;
  var end = options.end;
  if (start === end) {
    var emptyStream = new PassThrough();
    setImmediate(function() {
      emptyStream.end();
    });
    return emptyStream;
  }
  var stream = this._readStreamForRange(start, end);

  var destroyed = false;
  var refUnrefFilter = new RefUnrefFilter(this);
  stream.on("error", function(err) {
    setImmediate(function() {
      if (!destroyed) refUnrefFilter.emit("error", err);
    });
  });
  refUnrefFilter.destroy = function() {
    stream.unpipe(refUnrefFilter);
    refUnrefFilter.unref();
    stream.destroy();
  };

  var byteCounter = new AssertByteCountStream(end - start);
  refUnrefFilter.on("error", function(err) {
    setImmediate(function() {
      if (!destroyed) byteCounter.emit("error", err);
    });
  });
  byteCounter.destroy = function() {
    destroyed = true;
    refUnrefFilter.unpipe(byteCounter);
    refUnrefFilter.destroy();
  };

  return stream.pipe(refUnrefFilter).pipe(byteCounter);
}
```
- example usage
```shell
...
  // since we're dealing with an unsigned offset plus an unsigned size,
  // we only have 1 thing to check for.
  if (fileDataEnd > self.fileSize) {
    return callback(new Error("file data overflows file bounds: " +
        fileDataStart + " + " + entry.compressedSize + " > " + self.fileSize));
  }
}
var readStream = self.reader.createReadStream({start: fileDataStart, end: fileDataEnd});
var endpointStream = readStream;
if (compressed) {
  var destroyed = false;
  var inflateFilter = zlib.createInflateRaw();
  readStream.on("error", function(err) {
    // setImmediate here because errors can be emitted during the first call to pipe()
    setImmediate(function() {
...
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype.read"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>read (buffer, offset, length, position, callback)](#apidoc.element.yauzl.RandomAccessReader.prototype.read)
- description and source-code
```javascript
read = function (buffer, offset, length, position, callback) {
  var readStream = this.createReadStream({start: position, end: position + length});
  var writeStream = new Writable();
  var written = 0;
  writeStream._write = function(chunk, encoding, cb) {
    chunk.copy(buffer, offset + written, 0, chunk.length);
    written += chunk.length;
    cb();
  };
  writeStream.on("finish", callback);
  readStream.on("error", function(error) {
    callback(error);
  });
  readStream.pipe(writeStream);
}
```
- example usage
```shell
...
If you never call 'readStream.destroy()', then streams returned from this method do not need to implement a method '.destroy()'.
'.destroy()' should abort any streaming that is in progress and clean up any associated resources.
'.destroy()' will only be called after the stream has been 'unpipe()'d from its destination.

Note that the stream returned from this method might not be the same object that is provided by 'openReadStream()'.
The stream returned from this method might be 'pipe()'d through one or more filter streams (for example, a zlib inflate stream).

#### randomAccessReader.read(buffer, offset, length, position, callback)

Subclasses may implement this method.
The default implementation uses 'createReadStream()' to fill the 'buffer'.

This method should behave like 'fs.read()'.

#### randomAccessReader.close(callback)
...
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype.ref"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>ref ()](#apidoc.element.yauzl.RandomAccessReader.prototype.ref)
- description and source-code
```javascript
ref = function () {
  this.refCount += 1;
}
```
- example usage
```shell
...
if (callback == null) callback = defaultCallback;
if (typeof totalSize !== "number") throw new Error("expected totalSize parameter to be a number");
if (totalSize > Number.MAX_SAFE_INTEGER) {
  throw new Error("zip file too large. only file sizes up to 2^52 are supported due to JavaScript's Number type being an IEEE 754
 double.");
}

// the matching unref() call is in zipfile.close()
reader.ref();

// eocdr means End of Central Directory Record.
// search backwards for the eocdr signature.
// the last field of the eocdr is a variable-length comment.
// the comment size is encoded in a 2-byte field in the eocdr, which we can't find without trudging backwards through the comment
 to find it.
// as a consequence of this design decision, it's possible to have ambiguous zip file metadata if a coherent eocdr was in the comment
.
// we search backwards for a eocdr signature, and hope that whoever made the zip file was smart enough to forbid the eocdr signature
 in the comment.
...
```

#### <a name="apidoc.element.yauzl.RandomAccessReader.prototype.unref"></a>[function <span class="apidocSignatureSpan">yauzl.RandomAccessReader.prototype.</span>unref ()](#apidoc.element.yauzl.RandomAccessReader.prototype.unref)
- description and source-code
```javascript
unref = function () {
  var self = this;
  self.refCount -= 1;

  if (self.refCount > 0) return;
  if (self.refCount < 0) throw new Error("invalid unref");

  self.close(onCloseDone);

  function onCloseDone(err) {
    if (err) return self.emit('error', err);
    self.emit('close');
  }
}
```
- example usage
```shell
...
  self.emittedError = false;

  if (!self.lazyEntries) self.readEntry();
}
ZipFile.prototype.close = function() {
  if (!this.isOpen) return;
  this.isOpen = false;
  this.reader.unref();
};

function emitErrorAndAutoClose(self, err) {
  if (self.autoClose) self.close();
  emitError(self, err);
}
function emitError(self, err) {
...
```



# <a name="apidoc.module.yauzl.ZipFile"></a>[module yauzl.ZipFile](#apidoc.module.yauzl.ZipFile)

#### <a name="apidoc.element.yauzl.ZipFile.ZipFile"></a>[function <span class="apidocSignatureSpan">yauzl.</span>ZipFile (reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings)](#apidoc.element.yauzl.ZipFile.ZipFile)
- description and source-code
```javascript
function ZipFile(reader, centralDirectoryOffset, fileSize, entryCount, comment, autoClose, lazyEntries, decodeStrings) {
  var self = this;
  EventEmitter.call(self);
  self.reader = reader;
  // forward close events
  self.reader.on("error", function(err) {
    // error closing the fd
    emitError(self, err);
  });
  self.reader.once("close", function() {
    self.emit("close");
  });
  self.readEntryCursor = centralDirectoryOffset;
  self.fileSize = fileSize;
  self.entryCount = entryCount;
  self.comment = comment;
  self.entriesRead = 0;
  self.autoClose = !!autoClose;
  self.lazyEntries = !!lazyEntries;
  self.decodeStrings = !!decodeStrings;
  self.isOpen = true;
  self.emittedError = false;

  if (!self.lazyEntries) self.readEntry();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yauzl.ZipFile.super_"></a>[function <span class="apidocSignatureSpan">yauzl.ZipFile.</span>super_ ()](#apidoc.element.yauzl.ZipFile.super_)
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



# <a name="apidoc.module.yauzl.ZipFile.prototype"></a>[module yauzl.ZipFile.prototype](#apidoc.module.yauzl.ZipFile.prototype)

#### <a name="apidoc.element.yauzl.ZipFile.prototype.close"></a>[function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>close ()](#apidoc.element.yauzl.ZipFile.prototype.close)
- description and source-code
```javascript
close = function () {
  if (!this.isOpen) return;
  this.isOpen = false;
  this.reader.unref();
}
```
- example usage
```shell
...

'options' may be omitted or 'null'. The defaults are '{autoClose: true, lazyEntries: false, decodeStrings: true}'.

'autoClose' is effectively equivalent to:

'''js
zipfile.once("end", function() {
  zipfile.close();
});
'''

'lazyEntries' indicates that entries should be read only when 'readEntry()' is called.
If 'lazyEntries' is 'false', 'entry' events will be emitted as fast as possible to allow 'pipe()'ing
file data from all entries in parallel.
This is not recommended, as it can lead to out of control memory usage for zip files with many entries.
...
```

#### <a name="apidoc.element.yauzl.ZipFile.prototype.openReadStream"></a>[function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>openReadStream (entry, callback)](#apidoc.element.yauzl.ZipFile.prototype.openReadStream)
- description and source-code
```javascript
openReadStream = function (entry, callback) {
  var self = this;
  if (!self.isOpen) return callback(new Error("closed"));
  // make sure we don't lose the fd before we open the actual read stream
  self.reader.ref();
  var buffer = new Buffer(30);
  readAndAssertNoEof(self.reader, buffer, 0, buffer.length, entry.relativeOffsetOfLocalHeader, function(err) {
    try {
      if (err) return callback(err);
      // 0 - Local file header signature = 0x04034b50
      var signature = buffer.readUInt32LE(0);
      if (signature !== 0x04034b50) {
        return callback(new Error("invalid local file header signature: 0x" + signature.toString(16)));
      }
      // all this should be redundant
      // 4 - Version needed to extract (minimum)
      // 6 - General purpose bit flag
      // 8 - Compression method
      // 10 - File last modification time
      // 12 - File last modification date
      // 14 - CRC-32
      // 18 - Compressed size
      // 22 - Uncompressed size
      // 26 - File name length (n)
      var fileNameLength = buffer.readUInt16LE(26);
      // 28 - Extra field length (m)
      var extraFieldLength = buffer.readUInt16LE(28);
      // 30 - File name
      // 30+n - Extra field
      var localFileHeaderEnd = entry.relativeOffsetOfLocalHeader + buffer.length + fileNameLength + extraFieldLength;
      var compressed;
      if (entry.compressionMethod === 0) {
        // 0 - The file is stored (no compression)
        compressed = false;
      } else if (entry.compressionMethod === 8) {
        // 8 - The file is Deflated
        compressed = true;
      } else {
        return callback(new Error("unsupported compression method: " + entry.compressionMethod));
      }
      var fileDataStart = localFileHeaderEnd;
      var fileDataEnd = fileDataStart + entry.compressedSize;
      if (entry.compressedSize !== 0) {
        // bounds check now, because the read streams will probably not complain loud enough.
        // since we're dealing with an unsigned offset plus an unsigned size,
        // we only have 1 thing to check for.
        if (fileDataEnd > self.fileSize) {
          return callback(new Error("file data overflows file bounds: " +
              fileDataStart + " + " + entry.compressedSize + " > " + self.fileSize));
        }
      }
      var readStream = self.reader.createReadStream({start: fileDataStart, end: fileDataEnd});
      var endpointStream = readStream;
      if (compressed) {
        var destroyed = false;
        var inflateFilter = zlib.createInflateRaw();
        readStream.on("error", function(err) {
          // setImmediate here because errors can be emitted during the first call to pipe()
          setImmediate(function() {
            if (!destroyed) inflateFilter.emit("error", err);
          });
        });

        var checkerStream = new AssertByteCountStream(entry.uncompressedSize);
        inflateFilter.on("error", function(err) {
          // forward zlib errors to the client-visible stream
          setImmediate(function() {
            if (!destroyed) checkerStream.emit("error", err);
          });
        });
        checkerStream.destroy = function() {
          destroyed = true;
          inflateFilter.unpipe(checkerStream);
          readStream.unpipe(inflateFilter);
          // TODO: the inflateFilter now causes a memory leak. see Issue #27.
          readStream.destroy();
        };
        endpointStream = readStream.pipe(inflateFilter).pipe(checkerStream);
      }
      callback(null, endpointStream);
    } finally {
      self.reader.unref();
    }
  });
}
```
- example usage
```shell
...
  // directory file names end with '/'
  mkdirp(entry.fileName, function(err) {
    if (err) throw err;
    zipfile.readEntry();
  });
} else {
  // file entry
  zipfile.openReadStream(entry, function(err, readStream) {
    if (err) throw err;
    // ensure parent directory exists
    mkdirp(path.dirname(entry.fileName), function(err) {
      if (err) throw err;
      readStream.pipe(fs.createWriteStream(entry.fileName));
      readStream.on("end", function() {
        zipfile.readEntry();
...
```

#### <a name="apidoc.element.yauzl.ZipFile.prototype.readEntry"></a>[function <span class="apidocSignatureSpan">yauzl.ZipFile.prototype.</span>readEntry ()](#apidoc.element.yauzl.ZipFile.prototype.readEntry)
- description and source-code
```javascript
readEntry = function () {
  var self = this;
  if (self.entryCount === self.entriesRead) {
    // done with metadata
    setImmediate(function() {
      if (self.autoClose) self.close();
      if (self.emittedError) return;
      self.emit("end");
    });
    return;
  }
  if (self.emittedError) return;
  var buffer = new Buffer(46);
  readAndAssertNoEof(self.reader, buffer, 0, buffer.length, self.readEntryCursor, function(err) {
    if (err) return emitErrorAndAutoClose(self, err);
    if (self.emittedError) return;
    var entry = new Entry();
    // 0 - Central directory file header signature
    var signature = buffer.readUInt32LE(0);
    if (signature !== 0x02014b50) return emitErrorAndAutoClose(self, new Error("invalid central directory file header signature:
0x" + signature.toString(16)));
    // 4 - Version made by
    entry.versionMadeBy = buffer.readUInt16LE(4);
    // 6 - Version needed to extract (minimum)
    entry.versionNeededToExtract = buffer.readUInt16LE(6);
    // 8 - General purpose bit flag
    entry.generalPurposeBitFlag = buffer.readUInt16LE(8);
    // 10 - Compression method
    entry.compressionMethod = buffer.readUInt16LE(10);
    // 12 - File last modification time
    entry.lastModFileTime = buffer.readUInt16LE(12);
    // 14 - File last modification date
    entry.lastModFileDate = buffer.readUInt16LE(14);
    // 16 - CRC-32
    entry.crc32 = buffer.readUInt32LE(16);
    // 20 - Compressed size
    entry.compressedSize = buffer.readUInt32LE(20);
    // 24 - Uncompressed size
    entry.uncompressedSize = buffer.readUInt32LE(24);
    // 28 - File name length (n)
    entry.fileNameLength = buffer.readUInt16LE(28);
    // 30 - Extra field length (m)
    entry.extraFieldLength = buffer.readUInt16LE(30);
    // 32 - File comment length (k)
    entry.fileCommentLength = buffer.readUInt16LE(32);
    // 34 - Disk number where file starts
    // 36 - Internal file attributes
    entry.internalFileAttributes = buffer.readUInt16LE(36);
    // 38 - External file attributes
    entry.externalFileAttributes = buffer.readUInt32LE(38);
    // 42 - Relative offset of local file header
    entry.relativeOffsetOfLocalHeader = buffer.readUInt32LE(42);

    self.readEntryCursor += 46;

    buffer = new Buffer(entry.fileNameLength + entry.extraFieldLength + entry.fileCommentLength);
    readAndAssertNoEof(self.reader, buffer, 0, buffer.length, self.readEntryCursor, function(err) {
      if (err) return emitErrorAndAutoClose(self, err);
      if (self.emittedError) return;
      // 46 - File name
      var isUtf8 = (entry.generalPurposeBitFlag & 0x800) !== 0;
      entry.fileName = self.decodeStrings ? decodeBuffer(buffer, 0, entry.fileNameLength, isUtf8)
                                          : buffer.slice(0, entry.fileNameLength);

      // 46+n - Extra field
      var fileCommentStart = entry.fileNameLength + entry.extraFieldLength;
      var extraFieldBuffer = buffer.slice(entry.fileNameLength, fileCommentStart);
      entry.extraFields = [];
      var i = 0;
      while (i < extraFieldBuffer.length - 3) {
        var headerId = extraFieldBuffer.readUInt16LE(i + 0);
        var dataSize = extraFieldBuffer.readUInt16LE(i + 2);
        var dataStart = i + 4;
        var dataEnd = dataStart + dataSize;
        if (dataEnd > extraFieldBuffer.length) return emitErrorAndAutoClose(self, new Error("extra field length exceeds extra field
 buffer size"));
        var dataBuffer = new Buffer(dataSize);
        extraFieldBuffer.copy(dataBuffer, 0, dataStart, dataEnd);
        entry.extraFields.push({
          id: headerId,
          data: dataBuffer,
        });
        i = dataEnd;
      }

      // 46+n+m - File comment
      entry.fileComment = self.decodeStrings ? decodeBuffer(buffer, fileCommentStart, fileCommentStart + entry.fileCommentLength
, isUtf8)
                                             : buffer.slice(fileCommentStart, fileCommentStart + entry.fileCommentLength);
      // compatibility hack for https://github.com/thejoshwolfe/yauzl/issues/47
      entry.comment = entry.fileComment;

      self.readEntryCursor += b ...
```
- example usage
```shell
...
var yauzl = require("yauzl");
var fs = require("fs");
var path = require("path");
var mkdirp = require("mkdirp"); // or similar

yauzl.open("path/to/file.zip", {lazyEntries: true}, function(err, zipfile) {
if (err) throw err;
zipfile.readEntry();
zipfile.on("entry", function(entry) {
  if (/\/$/.test(entry.fileName)) {
    // directory file names end with '/'
    mkdirp(entry.fileName, function(err) {
      if (err) throw err;
      zipfile.readEntry();
    });
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
