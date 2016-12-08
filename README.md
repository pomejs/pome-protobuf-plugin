pome-protobuf-plugin
====================

pome-protobuf-plugin is a plugin for pome, it can be used in pome(>=0.9).

pome-protobuf-plugin provides messages encode&decode service for pome, and it uses [ProtoBuf.js](https://github.com/dcodeIO/ProtoBuf.js) to do this thing.

##Installation

```
npm install pome-protobuf-plugin
```

##Usage

the protos file should use json format, for it would be compatible for pome-protobuf. If you use proto file, you can use ProtoBuf.js to turn it to json file.

the default protos files are /config/serversProtos.json and /config/clientProtos.json, and you can specify your own protos files.


```
var protobuf = require('pome-protobuf-plugin');

	app.use(protobuf, {
		protobuf: {
			// serverProtos: /yourprotofilepath/
			// clientProtos: /yourprotofilepath/
		}
	});

```
