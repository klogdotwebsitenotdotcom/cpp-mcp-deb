# Packaged for .deb based systems

## To install 

```

cd cpp-mcp && dpkg-buildpackage -us -uc

# Go to back and install the .deb

cd .. && dpkg-deb -I ../libcpp-mcp-dev_*.deb

```

#### It should be installed on your system now to link against / use it

``` 

g++ -lmcp agent_example.cpp

```
