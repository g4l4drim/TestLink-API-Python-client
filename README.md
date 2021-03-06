TestLink API Python Client
==========================

Copyright 2011-2012 
James Stock, Olivier Renault, TestLink-API-Python-client developers

License [Apache License 2.0]

Introduction
------------

TestLink-API-Python-client is a Python XMLRPC client for the [TestLink API].

It's a brick of Olivier Renault [JinFeng] idea - an interaction of [TestLink], 
 [Robot Framework] and [Jenkins].

Initially based on the James Stock testlink-api-python-client R7.


Directory Layout
----------------

src/
*   Source for TestLink API Python Client

tests/
*   Unit Tests for TestLink API Python Client

examples/
*   Examples, how to use the TestLink API Python Client

Installation
------------

### Install TestLinkAPI into a virtualenv environment

```
[PYTHON27]\Scripts\virtualenv [PYENV]\testlink
[PYENV]\testlink\Scripts\activate
python setup.py install
```

### Run example with command line arguments

```
[PYENV]\testlink\Scripts\activate
python example\TestLinkExample.py 
               --server_url http://[YOURSERVER]/testlink/lib/api/xmlrpc.php
               --devKey [Users devKey generated by TestLink]
```

### Run unittests with TestLink Server interaction

```
[PYENV]\testlink\Scripts\activate
set TESTLINK_API_PYTHON_SERVER_URL=http://[YOURSERVER]/testlink/lib/api/xmlrpc.php
set TESTLINK_API_PYTHON_DEVKEY=[Users devKey generated by TestLink]
cd test\utest
python -m unittest testlinkapicallservertest testlinkapi_online_test
```

### Run unittests without TestLink Server interaction

```
[PYENV]\testlink\Scripts\activate
cd test\utest
python -m unittest testlinkhelpertest testlinkapi_offline_test
```


Download
--------

see [downloads]


TestLink-API-Python-client developers
-------------------------------------
*   [James Stock], [Olivier Renault], kereval.com
*   [g4l4drim], [pade], [lczub] 
*   anyone forgotten?


[Apache License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
[JinFeng]: http://www.sqaopen.net/blog/en/?p=63
[TestLink API]: http://www.teamst.org/_tldoc/1.8/phpdoc_api/TestlinkAPI/TestlinkXMLRPCServer.html
[TestLink]: http://www.teamst.org/
[Robot Framework]: http://code.google.com/p/robotframework
[Jenkins]: http://jenkins-ci.org/
[downloads]: https://github.com/lczub/TestLink-API-Python-client/downloads
[Olivier Renault]: https://github.com/orenault/TestLink-API-Python-client
[pade]: https://github.com/pade/TestLink-API-Python-client
[g4l4drim]: https://github.com/g4l4drim/TestLink-API-Python-client
[James Stock]: https://code.google.com/p/testlink-api-python-client/
[lczub]: https://github.com/lczub/TestLink-API-Python-client
