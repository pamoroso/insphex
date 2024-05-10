# Insphex

Insphex is a hex dump tool that shows the contents of files as a list of hexadecimal values and the correspnding ASCII characters. The program is written in Common Lisp and Interlisp, runs on the [Medley Interlisp](https://interlisp.org) environment, and is similar to the Linux tool `hexdump`.

![Insphex output window](https://raw.githubusercontent.com/pamoroso/insphex/main/insphex.png)


## Installation

Download the file `INSPHEX` from the project repo, copy it to a file system location your Medley system has access to, and optionally compile the source by evaluating the following expression at a Common Lisp Exec such as the XCL Exec:

```
(compile-file "INSPHEX")
```

Next, to load the program evaluate:

```lisp
(load "INSPHEX.DFASL")
```

or:

```lisp
(il:filesload insphex)
```


## Usage

Once Insphex is loaded you can call the following functions and commands.


### `HEXDUMP`

To run the program evaluate:

```lisp
(INSPHEX:HEXDUMP FILENAME)
```

where `FILENAME` is a file name. The function `INSHPEX` is exported from package `INSPHEX` with nickname `HX`.

The output goes to `*standard-output*`.


## Release history

See the [list of releases](https://github.com/pamoroso/insphex/releases) for notes on the changes in each version.


## Learn more

- [hex dump](https://en.wikipedia.org/wiki/Hex_dump)
- [Medley Interlisp](https://interlisp.org)


## Author

Insphex is developed by [Paolo Amoroso](https://github.com/pamoroso).


## License

This code is distributed under the MIT license, see the `LICENSE` file.
