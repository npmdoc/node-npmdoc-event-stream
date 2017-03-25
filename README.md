# api documentation for  [event-stream (v3.3.4)](http://github.com/dominictarr/event-stream)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-event-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-event-stream)
#### construct pipes of streams of events

[![NPM](https://nodei.co/npm/event-stream.png?downloads=true)](https://www.npmjs.com/package/event-stream)

[![apidoc](https://npmdoc.github.io/node-npmdoc-event-stream/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-event_stream_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-event-stream/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-event-stream/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Dominic Tarr",
        "email": "dominic.tarr@gmail.com",
        "url": "http://bit.ly/dominictarr"
    },
    "bugs": {
        "url": "https://github.com/dominictarr/event-stream/issues"
    },
    "dependencies": {
        "duplexer": "~0.1.1",
        "from": "~0",
        "map-stream": "~0.1.0",
        "pause-stream": "0.0.11",
        "split": "0.3",
        "stream-combiner": "~0.0.4",
        "through": "~2.3.1"
    },
    "description": "construct pipes of streams of events",
    "devDependencies": {
        "asynct": "*",
        "it-is": "1",
        "stream-spec": "~0.3.5",
        "tape": "~2.3.0",
        "ubelt": "~3.2.2"
    },
    "directories": {},
    "dist": {
        "shasum": "4ab4c9a0f5a54db9338b4c34d86bfce8f4b35571",
        "tarball": "https://registry.npmjs.org/event-stream/-/event-stream-3.3.4.tgz"
    },
    "gitHead": "0d9d45744b06ead81976b3400569160b76299a41",
    "homepage": "http://github.com/dominictarr/event-stream",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dominictarr",
            "email": "dominic.tarr@gmail.com"
        }
    ],
    "name": "event-stream",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/dominictarr/event-stream.git"
    },
    "scripts": {
        "prepublish": "npm ls && npm test",
        "test": "asynct test/",
        "test_tap": "set -e; for t in test/*.js; do node $t; done"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": {
            "ie": [
                8,
                9
            ],
            "firefox": [
                13
            ],
            "chrome": [
                20
            ],
            "safari": [
                5.1
            ],
            "opera": [
                12
            ]
        }
    },
    "version": "3.3.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module event-stream](#apidoc.module.event-stream)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>Stream ()](#apidoc.element.event-stream.Stream)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>child (child)](#apidoc.element.event-stream.child)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>concat ()](#apidoc.element.event-stream.concat)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>connect ()](#apidoc.element.event-stream.connect)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>duplex (writer, reader)](#apidoc.element.event-stream.duplex)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>from (source)](#apidoc.element.event-stream.from)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>join (str)](#apidoc.element.event-stream.join)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>log (name)](#apidoc.element.event-stream.log)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>map (mapper, opts)](#apidoc.element.event-stream.map)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>mapSync (sync)](#apidoc.element.event-stream.mapSync)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>merge ()](#apidoc.element.event-stream.merge)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>parse (options)](#apidoc.element.event-stream.parse)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>pause (write, end, opts)](#apidoc.element.event-stream.pause)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>pipe ()](#apidoc.element.event-stream.pipe)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>pipeable ()](#apidoc.element.event-stream.pipeable)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>pipeline ()](#apidoc.element.event-stream.pipeline)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>readArray (array)](#apidoc.element.event-stream.readArray)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>readable (func, continueOnError)](#apidoc.element.event-stream.readable)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>replace (from, to)](#apidoc.element.event-stream.replace)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>split (matcher, mapper, options)](#apidoc.element.event-stream.split)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>stringify ()](#apidoc.element.event-stream.stringify)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>through (write, end, opts)](#apidoc.element.event-stream.through)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>wait (callback)](#apidoc.element.event-stream.wait)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>writeArray (done)](#apidoc.element.event-stream.writeArray)

#### [module event-stream.through](#apidoc.module.event-stream.through)
1.  [function <span class="apidocSignatureSpan">event-stream.</span>through (write, end, opts)](#apidoc.element.event-stream.through.through)



# <a name="apidoc.module.event-stream"></a>[module event-stream](#apidoc.module.event-stream)

#### <a name="apidoc.element.event-stream.Stream"></a>[function <span class="apidocSignatureSpan">event-stream.</span>Stream ()](#apidoc.element.event-stream.Stream)
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

#### <a name="apidoc.element.event-stream.child"></a>[function <span class="apidocSignatureSpan">event-stream.</span>child (child)](#apidoc.element.event-stream.child)
- description and source-code
```javascript
child = function (child) {

  return es.duplex(child.stdin, child.stdout)

}
```
- example usage
```shell
...
## child (child_process)

Create a through stream from a child process ...

''' js
  var cp = require('child_process')

  es.child(cp.exec('grep Stream')) // a through stream

'''

## wait (callback)

waits for stream to emit 'end'.
joins chunks of a stream into a single string or buffer.
...
```

#### <a name="apidoc.element.event-stream.concat"></a>[function <span class="apidocSignatureSpan">event-stream.</span>concat ()](#apidoc.element.event-stream.concat)
- description and source-code
```javascript
concat = function () {
  var toMerge = [].slice.call(arguments)
  if (toMerge.length === 1 && (toMerge[0] instanceof Array)) {
    toMerge = toMerge[0] //handle array as arguments object
  }
  var stream = new Stream()
  stream.setMaxListeners(0) // allow adding more than 11 streams
  var endCount = 0
  stream.writable = stream.readable = true

  if (toMerge.length) {
    toMerge.forEach(function (e) {
      e.pipe(stream, {end: false})
      var ended = false
      e.on('end', function () {
        if(ended) return
        ended = true
        endCount ++
        if(endCount == toMerge.length)
          stream.emit('end')
      })
    })
  } else {
    process.nextTick(function () {
      stream.emit('end')
    })
  }

  stream.write = function (data) {
    this.emit('data', data)
  }
  stream.destroy = function () {
    toMerge.forEach(function (e) {
      if(e.destroy) e.destroy()
    })
  }
  return stream
}
```
- example usage
```shell
...
// wait. callback when 'end' is emitted, with all chunks appended as string.
//

es.wait = function (callback) {
  var arr = []
  return es.through(function (data) { arr.push(data) },
    function () {
      var body = Buffer.isBuffer(arr[0]) ? Buffer.concat(arr)
        : arr.join('')
      this.emit('data', body)
      this.emit('end')
      if(callback) callback(null, body)
    })
}
...
```

#### <a name="apidoc.element.event-stream.connect"></a>[function <span class="apidocSignatureSpan">event-stream.</span>connect ()](#apidoc.element.event-stream.connect)
- description and source-code
```javascript
connect = function () {

  var streams = [].slice.call(arguments)
    , first = streams[0]
    , last = streams[streams.length - 1]
    , thepipe = duplexer(first, last)

  if(streams.length == 1)
    return streams[0]
  else if (!streams.length)
    throw new Error('connect called with empty args')

  //pipe all the streams together

  function recurse (streams) {
    if(streams.length < 2)
      return
    streams[0].pipe(streams[1])
    recurse(streams.slice(1))
  }

  recurse(streams)

  function onerror () {
    var args = [].slice.call(arguments)
    args.unshift('error')
    thepipe.emit.apply(thepipe, args)
  }

  //es.duplex already reemits the error from the first and last stream.
  //add a listener for the inner streams in the pipeline.
  for(var i = 1; i < streams.length - 1; i ++)
    streams[i].on('error', onerror)

  return thepipe
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.event-stream.duplex"></a>[function <span class="apidocSignatureSpan">event-stream.</span>duplex (writer, reader)](#apidoc.element.event-stream.duplex)
- description and source-code
```javascript
function duplex(writer, reader) {
    var stream = new Stream()
    var ended = false

    forEach(writeMethods, proxyWriter)

    forEach(readMethods, proxyReader)

    forEach(readEvents, proxyStream)

    reader.on("end", handleEnd)

    writer.on("drain", function() {
      stream.emit("drain")
    })

    writer.on("error", reemit)
    reader.on("error", reemit)

    stream.writable = writer.writable
    stream.readable = reader.readable

    return stream

    function proxyWriter(methodName) {
        stream[methodName] = method

        function method() {
            return writer[methodName].apply(writer, arguments)
        }
    }

    function proxyReader(methodName) {
        stream[methodName] = method

        function method() {
            stream.emit(methodName)
            var func = reader[methodName]
            if (func) {
                return func.apply(reader, arguments)
            }
            reader.emit(methodName)
        }
    }

    function proxyStream(methodName) {
        reader.on(methodName, reemit)

        function reemit() {
            var args = slice.call(arguments)
            args.unshift(methodName)
            stream.emit.apply(stream, args)
        }
    }

    function handleEnd() {
        if (ended) {
            return
        }
        ended = true
        var args = slice.call(arguments)
        args.unshift("end")
        stream.emit.apply(stream, args)
    }

    function reemit(err) {
        stream.emit("error", err)
    }
}
```
- example usage
```shell
...

//
// child -- pipe through a child process
//

es.child = function (child) {

  return es.duplex(child.stdin, child.stdout)

}

//
// parse
//
// must be used after es.split() to ensure that each chunk represents a line
...
```

#### <a name="apidoc.element.event-stream.from"></a>[function <span class="apidocSignatureSpan">event-stream.</span>from (source)](#apidoc.element.event-stream.from)
- description and source-code
```javascript
function from(source) {
  if(Array.isArray(source)) {
		var source_index = 0, source_len = source.length;
    return from (function (i) {
      if(source_index < source_len)
        this.emit('data', source[source_index++])
      else
        this.emit('end')
      return true
    })
  }
  var s = new Stream(), i = 0
  s.ended = false
  s.started = false
  s.readable = true
  s.writable = false
  s.paused = false
  s.ended = false
  s.pause = function () {
    s.started = true
    s.paused = true
  }
  function next () {
    s.started = true
    if(s.ended) return
    while(!s.ended && !s.paused && source.call(s, i++, function () {
      if(!s.ended && !s.paused)
          process.nextTick(next);
    }))
      ;
  }
  s.resume = function () {
    s.started = true
    s.paused = false
    next()
  }
  s.on('end', function () {
    s.ended = true
    s.readable = false
    process.nextTick(s.destroy)
  })
  s.destroy = function () {
    s.ended = true
    s.emit('close')
  }
<span class="apidocCodeCommentSpan">  /*
    by default, the stream will start emitting at nextTick
    if you want, you can pause it, after pipeing.
    you can also resume before next tick, and that will also
    work.
  */
</span>  process.nextTick(function () {
    if(!s.started) s.resume()
  })
  return s
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.event-stream.join"></a>[function <span class="apidocSignatureSpan">event-stream.</span>join (str)](#apidoc.element.event-stream.join)
- description and source-code
```javascript
join = function (str) {

  //legacy api
  if('function' === typeof str)
    return es.wait(str)

  var first = true
  return es.through(function (data) {
    if(!first)
      this.emit('data', str)
    first = false
    this.emit('data', data)
    return true
  })
}
```
- example usage
```shell
...
    return JSON.stringify(Buffer.isBuffer(e) ? e.toString() : e) + '\n'
  })
}

//
// replace a string within a stream.
//
// warn: just concatenates the string and then does str.split().join().
// probably not optimal.
// for smallish responses, who cares?
// I need this for shadow-npm so it's only relatively small json files.

es.replace = function (from, to) {
  return es.pipeline(es.split(from), es.join(to))
}
...
```

#### <a name="apidoc.element.event-stream.log"></a>[function <span class="apidocSignatureSpan">event-stream.</span>log (name)](#apidoc.element.event-stream.log)
- description and source-code
```javascript
log = function (name) {
  return es.through(function (data) {
    var args = [].slice.call(arguments)
    if(name) console.error(name, data)
    else     console.error(data)
    this.emit('data', data)
  })
}
```
- example usage
```shell
...
a single data event with the reduced value once the input stream ends.

''' js
var reduce = require("stream-reduce");
process.stdin.pipe(reduce(function(acc, data) {
  return acc + data.length;
}, 0)).on("data", function(length) {
  console.log("stdin size:", length);
});
'''
...
```

#### <a name="apidoc.element.event-stream.map"></a>[function <span class="apidocSignatureSpan">event-stream.</span>map (mapper, opts)](#apidoc.element.event-stream.map)
- description and source-code
```javascript
map = function (mapper, opts) {

  var stream = new Stream()
    , self = this
    , inputs = 0
    , outputs = 0
    , ended = false
    , paused = false
    , destroyed = false
    , lastWritten = 0
    , inNext = false

  this.opts = opts || {};
  var errorEventName = this.opts.failures ? 'failure' : 'error';

  // Items that are not ready to be written yet (because they would come out of
  // order) get stuck in a queue for later.
  var writeQueue = {}

  stream.writable = true
  stream.readable = true

  function queueData (data, number) {
    var nextToWrite = lastWritten + 1

    if (number === nextToWrite) {
      // If it's next, and its not undefined write it
      if (data !== undefined) {
        stream.emit.apply(stream, ['data', data])
      }
      lastWritten ++
      nextToWrite ++
    } else {
      // Otherwise queue it for later.
      writeQueue[number] = data
    }

    // If the next value is in the queue, write it
    if (writeQueue.hasOwnProperty(nextToWrite)) {
      var dataToWrite = writeQueue[nextToWrite]
      delete writeQueue[nextToWrite]
      return queueData(dataToWrite, nextToWrite)
    }

    outputs ++
    if(inputs === outputs) {
      if(paused) paused = false, stream.emit('drain') //written all the incoming events
      if(ended) end()
    }
  }

  function next (err, data, number) {
    if(destroyed) return
    inNext = true

    if (!err || self.opts.failures) {
      queueData(data, number)
    }

    if (err) {
      stream.emit.apply(stream, [ errorEventName, err ]);
    }

    inNext = false;
  }

  // Wrap the mapper function by calling its callback with the order number of
  // the item in the stream.
  function wrappedMapper (input, number, callback) {
    return mapper.call(null, input, function(err, data){
      callback(err, data, number)
    })
  }

  stream.write = function (data) {
    if(ended) throw new Error('map stream is not writable')
    inNext = false
    inputs ++

    try {
      //catch sync errors and handle them like async errors
      var written = wrappedMapper(data, inputs, next)
      paused = (written === false)
      return !paused
    } catch (err) {
      //if the callback has been called syncronously, and the error
      //has occured in an listener, throw it again.
      if(inNext)
        throw err
      next(err)
      return !paused
    }
  }

  function end (data) {
    //if end was called with args, write it,
    ended = true //write will emit 'end' if ended is true
    stream.writable = false
    if(data !== undefined) {
      return queueData(data, inputs)
    } else if (inputs == outputs) { //wait for processing
      stream.readable = false, stream.emit('end'), stream.destroy()
    }
  }

  stream.end = function (data) {
    if(ended) return
    end()
  }

  stream.destroy = function () {
    ended = destroyed = true
    stream.writable = stream.readable = paused = false
    process.nextTick(function () {
      stream.emit('close')
    })
  }
  stream.pause = function () {
    paused = true
  }

  stream.resume = function () {
    paused = false
  }

  return stream
}
```
- example usage
```shell
...

if(!module.parent) {
  var es = require('event-stream')
  var inspect = require('util').inspect

  process.stdin                        //connect streams together with 'pipe'
    .pipe(es.split())                  //split stream to break on newlines
    .pipe(es.map(function (data, cb) { //turn this async function into a stream
      cb(null
        , inspect(JSON.parse(data)))   //render it nicely
    }))
    .pipe(process.stdout)              // pipe it to stdout !
}
'''
run it ...
...
```

#### <a name="apidoc.element.event-stream.mapSync"></a>[function <span class="apidocSignatureSpan">event-stream.</span>mapSync (sync)](#apidoc.element.event-stream.mapSync)
- description and source-code
```javascript
mapSync = function (sync) {
  return es.through(function write(data) {
    var mappedData
    try {
      mappedData = sync(data)
    } catch (err) {
      return this.emit('error', err)
    }
    if (mappedData !== undefined)
      this.emit('data', mappedData)
  })
}
```
- example usage
```shell
...
}
//
// stringify
//

es.stringify = function () {
  var Buffer = require('buffer').Buffer
  return es.mapSync(function (e){
    return JSON.stringify(Buffer.isBuffer(e) ? e.toString() : e) + '\n'
  })
}

//
// replace a string within a stream.
//
...
```

#### <a name="apidoc.element.event-stream.merge"></a>[function <span class="apidocSignatureSpan">event-stream.</span>merge ()](#apidoc.element.event-stream.merge)
- description and source-code
```javascript
merge = function () {
  var toMerge = [].slice.call(arguments)
  if (toMerge.length === 1 && (toMerge[0] instanceof Array)) {
    toMerge = toMerge[0] //handle array as arguments object
  }
  var stream = new Stream()
  stream.setMaxListeners(0) // allow adding more than 11 streams
  var endCount = 0
  stream.writable = stream.readable = true

  if (toMerge.length) {
    toMerge.forEach(function (e) {
      e.pipe(stream, {end: false})
      var ended = false
      e.on('end', function () {
        if(ended) return
        ended = true
        endCount ++
        if(endCount == toMerge.length)
          stream.emit('end')
      })
    })
  } else {
    process.nextTick(function () {
      stream.emit('end')
    })
  }

  stream.write = function (data) {
    this.emit('data', data)
  }
  stream.destroy = function () {
    toMerge.forEach(function (e) {
      if(e.destroy) e.destroy()
    })
  }
  return stream
}
```
- example usage
```shell
...
> concat → merge

Merges streams into one and returns it.
Incoming data will be emitted as soon it comes into - no ordering will be applied (for example: 'data1 data1 data2 data1 data2' -
where 'data1' and 'data2' is data from two streams).
Counts how many streams were passed to it and emits end only when all streams emitted end.

'''js
es.merge(
  process.stdout,
  process.stderr
).pipe(fs.createWriteStream('output.log'));
'''

It can also take an Array of streams as input like this:
'''js
...
```

#### <a name="apidoc.element.event-stream.parse"></a>[function <span class="apidocSignatureSpan">event-stream.</span>parse (options)](#apidoc.element.event-stream.parse)
- description and source-code
```javascript
parse = function (options) {
  var emitError = !!(options ? options.error : false)
  return es.through(function (data) {
    var obj
    try {
      if(data) //ignore empty lines
        obj = JSON.parse(data.toString())
    } catch (err) {
      if (emitError)
        return this.emit('error', err)
      return console.error(err, 'attempting to parse:', data)
    }
    //ignore lines that where only whitespace.
    if(obj !== undefined)
      this.emit('data', obj)
  })
}
```
- example usage
```shell
...

}

//
// parse
//
// must be used after es.split() to ensure that each chunk represents a line
// source.pipe(es.split()).pipe(es.parse())

es.parse = function (options) {
var emitError = !!(options ? options.error : false)
return es.through(function (data) {
  var obj
  try {
    if(data) //ignore empty lines
...
```

#### <a name="apidoc.element.event-stream.pause"></a>[function <span class="apidocSignatureSpan">event-stream.</span>pause (write, end, opts)](#apidoc.element.event-stream.pause)
- description and source-code
```javascript
function through(write, end, opts) {
  write = write || function (data) { this.queue(data) }
  end = end || function () { this.queue(null) }

  var ended = false, destroyed = false, buffer = [], _ended = false
  var stream = new Stream()
  stream.readable = stream.writable = true
  stream.paused = false

//  stream.autoPause   = !(opts && opts.autoPause   === false)
  stream.autoDestroy = !(opts && opts.autoDestroy === false)

  stream.write = function (data) {
    write.call(this, data)
    return !stream.paused
  }

  function drain() {
    while(buffer.length && !stream.paused) {
      var data = buffer.shift()
      if(null === data)
        return stream.emit('end')
      else
        stream.emit('data', data)
    }
  }

  stream.queue = stream.push = function (data) {
//    console.error(ended)
    if(_ended) return stream
    if(data === null) _ended = true
    buffer.push(data)
    drain()
    return stream
  }

  //this will be registered as the first 'end' listener
  //must call destroy next tick, to make sure we're after any
  //stream piped from here.
  //this is only a problem if end is not emitted synchronously.
  //a nicer way to do this is to make sure this is the last listener for 'end'

  stream.on('end', function () {
    stream.readable = false
    if(!stream.writable && stream.autoDestroy)
      process.nextTick(function () {
        stream.destroy()
      })
  })

  function _end () {
    stream.writable = false
    end.call(stream)
    if(!stream.readable && stream.autoDestroy)
      stream.destroy()
  }

  stream.end = function (data) {
    if(ended) return
    ended = true
    if(arguments.length) stream.write(data)
    _end() // will emit or queue
    return stream
  }

  stream.destroy = function () {
    if(destroyed) return
    destroyed = true
    ended = true
    buffer.length = 0
    stream.writable = stream.readable = false
    stream.emit('close')
    return stream
  }

  stream.pause = function () {
    if(stream.paused) return
    stream.paused = true
    return stream
  }

  stream.resume = function () {
    if(stream.paused) {
      stream.paused = false
      stream.emit('resume')
    }
    drain()
    //may have become paused again,
    //as drain emits 'data'.
    if(!stream.paused)
      stream.emit('drain')
    return stream
  }
  return stream
}
```
- example usage
```shell
...

[node Stream documentation](http://nodejs.org/api/stream.html)

## through (write?, end?)

Re-emits data synchronously. Easy way to create synchronous through streams.
Pass in optional 'write' and 'end' methods. They will be called in the
context of the stream. Use 'this.pause()' and 'this.resume()' to manage flow.
Check 'this.paused' to see current flow state. (write always returns '!this.paused')

this function is the basis for most of the synchronous streams in 'event-stream'.

''' js

es.through(function write(data) {
...
```

#### <a name="apidoc.element.event-stream.pipe"></a>[function <span class="apidocSignatureSpan">event-stream.</span>pipe ()](#apidoc.element.event-stream.pipe)
- description and source-code
```javascript
pipe = function () {

  var streams = [].slice.call(arguments)
    , first = streams[0]
    , last = streams[streams.length - 1]
    , thepipe = duplexer(first, last)

  if(streams.length == 1)
    return streams[0]
  else if (!streams.length)
    throw new Error('connect called with empty args')

  //pipe all the streams together

  function recurse (streams) {
    if(streams.length < 2)
      return
    streams[0].pipe(streams[1])
    recurse(streams.slice(1))
  }

  recurse(streams)

  function onerror () {
    var args = [].slice.call(arguments)
    args.unshift('error')
    thepipe.emit.apply(thepipe, args)
  }

  //es.duplex already reemits the error from the first and last stream.
  //add a listener for the inner streams in the pipeline.
  for(var i = 1; i < streams.length - 1; i ++)
    streams[i].on('error', onerror)

  return thepipe
}
```
- example usage
```shell
...
var stream = new Stream()
stream.setMaxListeners(0) // allow adding more than 11 streams
var endCount = 0
stream.writable = stream.readable = true

if (toMerge.length) {
  toMerge.forEach(function (e) {
    e.pipe(stream, {end: false})
    var ended = false
    e.on('end', function () {
      if(ended) return
      ended = true
      endCount ++
      if(endCount == toMerge.length)
        stream.emit('end')
...
```

#### <a name="apidoc.element.event-stream.pipeable"></a>[function <span class="apidocSignatureSpan">event-stream.</span>pipeable ()](#apidoc.element.event-stream.pipeable)
- description and source-code
```javascript
pipeable = function () {
  throw new Error('[EVENT-STREAM] es.pipeable is deprecated')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.event-stream.pipeline"></a>[function <span class="apidocSignatureSpan">event-stream.</span>pipeline ()](#apidoc.element.event-stream.pipeline)
- description and source-code
```javascript
pipeline = function () {

  var streams = [].slice.call(arguments)
    , first = streams[0]
    , last = streams[streams.length - 1]
    , thepipe = duplexer(first, last)

  if(streams.length == 1)
    return streams[0]
  else if (!streams.length)
    throw new Error('connect called with empty args')

  //pipe all the streams together

  function recurse (streams) {
    if(streams.length < 2)
      return
    streams[0].pipe(streams[1])
    recurse(streams.slice(1))
  }

  recurse(streams)

  function onerror () {
    var args = [].slice.call(arguments)
    args.unshift('error')
    thepipe.emit.apply(thepipe, args)
  }

  //es.duplex already reemits the error from the first and last stream.
  //add a listener for the inner streams in the pipeline.
  for(var i = 1; i < streams.length - 1; i ++)
    streams[i].on('error', onerror)

  return thepipe
}
```
- example usage
```shell
...
//
// warn: just concatenates the string and then does str.split().join().
// probably not optimal.
// for smallish responses, who cares?
// I need this for shadow-npm so it's only relatively small json files.

es.replace = function (from, to) {
  return es.pipeline(es.split(from), es.join(to))
}

//
// join chunks with a joiner. just like Array#join
// also accepts a callback that is passed the chunks appended together
// this is still supported for legacy reasons.
//
...
```

#### <a name="apidoc.element.event-stream.readArray"></a>[function <span class="apidocSignatureSpan">event-stream.</span>readArray (array)](#apidoc.element.event-stream.readArray)
- description and source-code
```javascript
readArray = function (array) {
  var stream = new Stream()
    , i = 0
    , paused = false
    , ended = false

  stream.readable = true
  stream.writable = false

  if(!Array.isArray(array))
    throw new Error('event-stream.read expects an array')

  stream.resume = function () {
    if(ended) return
    paused = false
    var l = array.length
    while(i < l && !paused && !ended) {
      stream.emit('data', array[i++])
    }
    if(i == l && !ended)
      ended = true, stream.readable = false, stream.emit('end')
  }
  process.nextTick(stream.resume)
  stream.pause = function () {
     paused = true
  }
  stream.destroy = function () {
    ended = true
    stream.emit('close')
  }
  return stream
}
```
- example usage
```shell
...

Create a readable stream from an Array.

Just emit each item as a data event, respecting 'pause' and 'resume'.

''' js
  var es = require('event-stream')
    , reader = es.readArray([1,2,3])

  reader.pipe(...)
'''

If you want the stream behave like a 0.10 stream you will need to wrap it using ['Readable.wrap()'](http://nodejs.org/api/stream
.html#stream_readable_wrap_stream) function. Example:

''' js
...
```

#### <a name="apidoc.element.event-stream.readable"></a>[function <span class="apidocSignatureSpan">event-stream.</span>readable (func, continueOnError)](#apidoc.element.event-stream.readable)
- description and source-code
```javascript
readable = function (func, continueOnError) {
  var stream = new Stream()
    , i = 0
    , paused = false
    , ended = false
    , reading = false

  stream.readable = true
  stream.writable = false

  if('function' !== typeof func)
    throw new Error('event-stream.readable expects async function')

  stream.on('end', function () { ended = true })

  function get (err, data) {

    if(err) {
      stream.emit('error', err)
      if(!continueOnError) stream.emit('end')
    } else if (arguments.length > 1)
      stream.emit('data', data)

    immediately(function () {
      if(ended || paused || reading) return
      try {
        reading = true
        func.call(stream, i++, function () {
          reading = false
          get.apply(null, arguments)
        })
      } catch (err) {
        stream.emit('error', err)
      }
    })
  }
  stream.resume = function () {
    paused = false
    get()
  }
  process.nextTick(get)
  stream.pause = function () {
     paused = true
  }
  stream.destroy = function () {
    stream.emit('end')
    stream.emit('close')
    ended = true
  }
  return stream
}
```
- example usage
```shell
...
create a readable stream (that respects pause) from an async function.
while the stream is not paused,
the function will be polled with '(count, callback)',
and 'this'  will be the readable stream.

''' js

es.readable(function (count, callback) {
if(streamHasEnded)
  return this.emit('end')

//...

this.emit('data', data) //use this way to emit multiple chunks per call.
...
```

#### <a name="apidoc.element.event-stream.replace"></a>[function <span class="apidocSignatureSpan">event-stream.</span>replace (from, to)](#apidoc.element.event-stream.replace)
- description and source-code
```javascript
replace = function (from, to) {
  return es.pipeline(es.split(from), es.join(to))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.event-stream.split"></a>[function <span class="apidocSignatureSpan">event-stream.</span>split (matcher, mapper, options)](#apidoc.element.event-stream.split)
- description and source-code
```javascript
function split(matcher, mapper, options) {
  var decoder = new Decoder()
  var soFar = ''
  var maxLength = options && options.maxLength;
  if('function' === typeof matcher)
    mapper = matcher, matcher = null
  if (!matcher)
    matcher = /\r?\n/

  function emit(stream, piece) {
    if(mapper) {
      try {
        piece = mapper(piece)
      }
      catch (err) {
        return stream.emit('error', err)
      }
      if('undefined' !== typeof piece)
        stream.queue(piece)
    }
    else
      stream.queue(piece)
  }

  function next (stream, buffer) {
    var pieces = ((soFar != null ? soFar : '') + buffer).split(matcher)
    soFar = pieces.pop()

    if (maxLength && soFar.length > maxLength)
      stream.emit('error', new Error('maximum buffer reached'))

    for (var i = 0; i < pieces.length; i++) {
      var piece = pieces[i]
      emit(stream, piece)
    }
  }

  return through(function (b) {
    next(this, decoder.write(b))
  },
  function () {
    if(decoder.end)
      next(this, decoder.end())
    if(soFar != null)
      emit(this, soFar)
    this.queue(null)
  })
}
```
- example usage
```shell
...
return es.duplex(child.stdin, child.stdout)

}

//
// parse
//
// must be used after es.split() to ensure that each chunk represents a line
// source.pipe(es.split()).pipe(es.parse())

es.parse = function (options) {
var emitError = !!(options ? options.error : false)
return es.through(function (data) {
  var obj
  try {
...
```

#### <a name="apidoc.element.event-stream.stringify"></a>[function <span class="apidocSignatureSpan">event-stream.</span>stringify ()](#apidoc.element.event-stream.stringify)
- description and source-code
```javascript
stringify = function () {
  var Buffer = require('buffer').Buffer
  return es.mapSync(function (e){
    return JSON.stringify(Buffer.isBuffer(e) ? e.toString() : e) + '\n'
  })
}
```
- example usage
```shell
...
//
// stringify
//

es.stringify = function () {
  var Buffer = require('buffer').Buffer
  return es.mapSync(function (e){
    return JSON.stringify(Buffer.isBuffer(e) ? e.toString() : e) + '\n'
  })
}

//
// replace a string within a stream.
//
// warn: just concatenates the string and then does str.split().join().
...
```

#### <a name="apidoc.element.event-stream.through"></a>[function <span class="apidocSignatureSpan">event-stream.</span>through (write, end, opts)](#apidoc.element.event-stream.through)
- description and source-code
```javascript
function through(write, end, opts) {
  write = write || function (data) { this.queue(data) }
  end = end || function () { this.queue(null) }

  var ended = false, destroyed = false, buffer = [], _ended = false
  var stream = new Stream()
  stream.readable = stream.writable = true
  stream.paused = false

//  stream.autoPause   = !(opts && opts.autoPause   === false)
  stream.autoDestroy = !(opts && opts.autoDestroy === false)

  stream.write = function (data) {
    write.call(this, data)
    return !stream.paused
  }

  function drain() {
    while(buffer.length && !stream.paused) {
      var data = buffer.shift()
      if(null === data)
        return stream.emit('end')
      else
        stream.emit('data', data)
    }
  }

  stream.queue = stream.push = function (data) {
//    console.error(ended)
    if(_ended) return stream
    if(data === null) _ended = true
    buffer.push(data)
    drain()
    return stream
  }

  //this will be registered as the first 'end' listener
  //must call destroy next tick, to make sure we're after any
  //stream piped from here.
  //this is only a problem if end is not emitted synchronously.
  //a nicer way to do this is to make sure this is the last listener for 'end'

  stream.on('end', function () {
    stream.readable = false
    if(!stream.writable && stream.autoDestroy)
      process.nextTick(function () {
        stream.destroy()
      })
  })

  function _end () {
    stream.writable = false
    end.call(stream)
    if(!stream.readable && stream.autoDestroy)
      stream.destroy()
  }

  stream.end = function (data) {
    if(ended) return
    ended = true
    if(arguments.length) stream.write(data)
    _end() // will emit or queue
    return stream
  }

  stream.destroy = function () {
    if(destroyed) return
    destroyed = true
    ended = true
    buffer.length = 0
    stream.writable = stream.readable = false
    stream.emit('close')
    return stream
  }

  stream.pause = function () {
    if(stream.paused) return
    stream.paused = true
    return stream
  }

  stream.resume = function () {
    if(stream.paused) {
      stream.paused = false
      stream.emit('resume')
    }
    drain()
    //may have become paused again,
    //as drain emits 'data'.
    if(!stream.paused)
      stream.emit('drain')
    return stream
  }
  return stream
}
```
- example usage
```shell
...


//
// map sync
//

es.mapSync = function (sync) {
return es.through(function write(data) {
  var mappedData
  try {
    mappedData = sync(data)
  } catch (err) {
    return this.emit('error', err)
  }
  if (mappedData !== undefined)
...
```

#### <a name="apidoc.element.event-stream.wait"></a>[function <span class="apidocSignatureSpan">event-stream.</span>wait (callback)](#apidoc.element.event-stream.wait)
- description and source-code
```javascript
wait = function (callback) {
  var arr = []
  return es.through(function (data) { arr.push(data) },
    function () {
      var body = Buffer.isBuffer(arr[0]) ? Buffer.concat(arr)
        : arr.join('')
      this.emit('data', body)
      this.emit('end')
      if(callback) callback(null, body)
    })
}
```
- example usage
```shell
...
// this is still supported for legacy reasons.
//

es.join = function (str) {

//legacy api
if('function' === typeof str)
  return es.wait(str)

var first = true
return es.through(function (data) {
  if(!first)
    this.emit('data', str)
  first = false
  this.emit('data', data)
...
```

#### <a name="apidoc.element.event-stream.writeArray"></a>[function <span class="apidocSignatureSpan">event-stream.</span>writeArray (done)](#apidoc.element.event-stream.writeArray)
- description and source-code
```javascript
writeArray = function (done) {
  if ('function' !== typeof done)
    throw new Error('function writeArray (done): done must be function')

  var a = new Stream ()
    , array = [], isDone = false
  a.write = function (l) {
    array.push(l)
  }
  a.end = function () {
    isDone = true
    done(null, array)
  }
  a.writable = true
  a.readable = false
  a.destroy = function () {
    a.writable = a.readable = false
    if(isDone) return
    done(new Error('destroyed before end'), array)
  }
  return a
}
```
- example usage
```shell
...

create a writeable stream from a callback,
all 'data' events are stored in an array, which is passed to the callback when the stream ends.

''' js
  var es = require('event-stream')
    , reader = es.readArray([1, 2, 3])
    , writer = es.writeArray(function (err, array){
      //array deepEqual [1, 2, 3]
    })

  reader.pipe(writer)
'''

## pause  ()
...
```



# <a name="apidoc.module.event-stream.through"></a>[module event-stream.through](#apidoc.module.event-stream.through)

#### <a name="apidoc.element.event-stream.through.through"></a>[function <span class="apidocSignatureSpan">event-stream.</span>through (write, end, opts)](#apidoc.element.event-stream.through.through)
- description and source-code
```javascript
function through(write, end, opts) {
  write = write || function (data) { this.queue(data) }
  end = end || function () { this.queue(null) }

  var ended = false, destroyed = false, buffer = [], _ended = false
  var stream = new Stream()
  stream.readable = stream.writable = true
  stream.paused = false

//  stream.autoPause   = !(opts && opts.autoPause   === false)
  stream.autoDestroy = !(opts && opts.autoDestroy === false)

  stream.write = function (data) {
    write.call(this, data)
    return !stream.paused
  }

  function drain() {
    while(buffer.length && !stream.paused) {
      var data = buffer.shift()
      if(null === data)
        return stream.emit('end')
      else
        stream.emit('data', data)
    }
  }

  stream.queue = stream.push = function (data) {
//    console.error(ended)
    if(_ended) return stream
    if(data === null) _ended = true
    buffer.push(data)
    drain()
    return stream
  }

  //this will be registered as the first 'end' listener
  //must call destroy next tick, to make sure we're after any
  //stream piped from here.
  //this is only a problem if end is not emitted synchronously.
  //a nicer way to do this is to make sure this is the last listener for 'end'

  stream.on('end', function () {
    stream.readable = false
    if(!stream.writable && stream.autoDestroy)
      process.nextTick(function () {
        stream.destroy()
      })
  })

  function _end () {
    stream.writable = false
    end.call(stream)
    if(!stream.readable && stream.autoDestroy)
      stream.destroy()
  }

  stream.end = function (data) {
    if(ended) return
    ended = true
    if(arguments.length) stream.write(data)
    _end() // will emit or queue
    return stream
  }

  stream.destroy = function () {
    if(destroyed) return
    destroyed = true
    ended = true
    buffer.length = 0
    stream.writable = stream.readable = false
    stream.emit('close')
    return stream
  }

  stream.pause = function () {
    if(stream.paused) return
    stream.paused = true
    return stream
  }

  stream.resume = function () {
    if(stream.paused) {
      stream.paused = false
      stream.emit('resume')
    }
    drain()
    //may have become paused again,
    //as drain emits 'data'.
    if(!stream.paused)
      stream.emit('drain')
    return stream
  }
  return stream
}
```
- example usage
```shell
...


//
// map sync
//

es.mapSync = function (sync) {
return es.through(function write(data) {
  var mappedData
  try {
    mappedData = sync(data)
  } catch (err) {
    return this.emit('error', err)
  }
  if (mappedData !== undefined)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
