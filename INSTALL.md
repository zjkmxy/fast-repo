# Submodules

Reposistory has a number of submodules it depends on, so clone using `--recursive` option.

# Dependencies

* [ndn-cpp](https://github.com/named-data/ndn-cpp/blob/master/INSTALL.md)
* [cpp-cnl](https://github.com/named-data/cnl-cpp/blob/master/INSTALL.md)
* [rocksdb](https://github.com/facebook/rocksdb/blob/master/INSTALL.md)
* protobuf
* boost

Compile these dependencies from source or use `brew` (`apt-get`) if aplicable.

```
brew install boost rocksdb protobuf
```

```
sudo apt-get install -y libboost-all-dev protobuf-compiler
```

# Build

Specify paths to dependencies in `CPPFLAGS` and `LDFLAGS` variables and configure & compile the project:

```
CPPFLAGS="..." LDFLAGS="..." ./configure 
make
```

