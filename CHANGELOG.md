Release 3.5.8


### Fixed Bugs:
* Remoting module has kept the same timeout,refer to [issue270](https://github.com/alibaba/RocketMQ/issues/270)
* Consume queue offset will not repeated when state transition over
* Client will not throw exception when broker is down
* Fix ordering message Deadlock problems   

### Optimize:
* Support max retry times in message deliver.context priority beyond consumer's. 
* Remove channel isWriteable check
* Some performance improvement 



Release 3.4.6

### Fixed Bugs:
* Repair HA thread resource leak bug when using telnet
* Repair negative offset problem

### Optimize:
* Update netty to 4.0.29 version
* Refactor message store module
* Replace native CRC alrightom with PureJavaCrc,thanks[@dltc](https://github.com/dltc)
* Optimize server network layer protocol.supports a variety of connected clients in a different way.
* Improve performance dramatically when message accumulation occur
* Add timeout parameter when invoking the command to query broker accumulation info
* Remove some useless tool class
* Add apache license Notice file


### New Features
* [Java SDK](https://help.aliyun.com/document_detail/29546.html?spm=5176.doc29546.3.3.FNzQoZ)
* [C++ SDK(Windows & Linux)](https://help.aliyun.com/document_detail/29555.html?spm=5176.doc29555.3.3.Yl0jA8)
* [.Net SDK](https://help.aliyun.com/document_detail/29561.html?spm=5176.doc29561.3.3.nIAzgT)

## Notice
* From 3.4.6 version, we strongly recommend guys to use the above SDKs. 100% compatible with RocketMQ native SDK.
* Nowadays, we have opened Java SDK source,you can get it from maven repository.we will continue to open C++ and .Net sources in the near future.

