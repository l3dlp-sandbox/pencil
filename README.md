# Pencil

A GUI prototyping tool for GNU/Linux, Windows & Mac.


## Status

This project was originally hosted on https://code.google.com/p/evoluspencil/ &
was abandoned around 2013. This fork was started for new development on March
13th, 2015.

Much of this project is still unmaintained & could use some love.


## Prerequisites

You will need version 36 or higher of `firefox` or `xulrunner` to run Pencil.


## Build

If you want to build for Firefox, or Mac pass `xpi` or `mac` to
`./build.sh`, respectively. It might work.

### Linux
```bash

cd build
./build.sh linux
xulrunner Outputs/Linux/application.ini || firefox --app Outputs/Linux/application.ini

```

### Windows
```bash

cd build
./build.sh win32
```

This should place an installer `exe` in `Outputs/`.


## Develop

If you set the `DEBUG` environmental variable, the `build.sh` script will
enable debugging settings, like printing calls to `dump()` to the console:
```bash

export DEBUG=true
cd build
./build.sh linux
xulrunner Outputs/Linux/application.ini -console

```


## License

This fork is released under GPLv2 like it's parent codebase.

http://pencil.evolus.vn/

https://code.google.com/p/evoluspencil/