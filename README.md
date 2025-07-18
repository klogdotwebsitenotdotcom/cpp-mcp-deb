# Packaged for .deb based systems

## To install 

```

mkdir ~/libmcp

# Debian does things a bit weird

cd ~/libmcp/ && git clone https://github.com/klogdotwebsitenotdotcom/cpp-mcp-deb.git

cd cpp-mcp-deb && dpkg-buildpackage -us -uc

# Now debian create some weird mess in ../

cd .. && dpkg-deb -I ./libcpp-mcp-dev_*.deb

# Or just install it from the current directory

dpkg-deb -I ../lib-mcp-dev_*.deb

```

#### It should be installed on your system now to link against / use it

``` 

g++ -lmcp agent_example.cpp

```
