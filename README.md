# Connext Professional (C API) - Accessing CharSeq elemenents 

This simple example is based on typical `rtiddsgen`-generated example, but adds some detail showing how to get and set CharSeq elements.

## Generating code and building the example

The instructions below assume that:
- The `NDDSHOME` environment variable is set to your Connext Professional installation directory
- *YOUR_ARCH* corresponds to the platform for which you will build, for example `x64Linux4gcc7.3.0` or `x64Darwin17clang9.0`

```
git clone https://github.com/dgochenour/sequence_c.git
cd sequence_c
$NDDSHOME/bin/rtiddsgen ./example.idl -ppDisable -language C -update typefiles -update makefiles -platform YOUR_ARCH
make -f make_example_<YOUR_ARCH>
```

## Runing the example

- In one terminal:
```
cd your/project/directory
./objs/<YOUR_ARCH>/example_publisher
```
- In a second terminal:
```
cd your/project/directory
./objs/<YOUR_ARCH>/example_subscriber
```