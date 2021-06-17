# LibET
Light library containing useful methods and utilities. Library also serves as a playground to experiment with my implementations of various algorithms and functionalities. Built to serve some of my other projects.

## **Functionalities of the Library**
The library lies under the global namespace `et::`. Under this namespace, the following components could be found:
- `et::parsing::commandline` - utilities for parsing the argc and argv argments that come from the commendline.
- `et::utils::string_utils` - helper functions and utilities for working with strings.

For detailed information on each component, Doxygen documentation could be generated by running the command `make docs`. From there, the documentation should exist in both Latex and HTML  forms in the `docs/doxygen/` directory.

## **Compiling LibET**
To setup and build LibET, run the Makefile as `make build`. This should create both a static archive and dynamic library named `libet.a` and `libet.so` respectively which could then be used in other projects along with the exposed public headers.

## **Running the Unit Tests**
Inside `tests/` there exists unit tests for each method in the library. By looking at the unit tests, it is also possible to see how each method functions. To run the unit tests:
1) Install the catch2 header and place it inside of libs/. This could be done manually or via script `setup.sh`.
2) Compile the unit tests by running `make test`.
3) Run the tests binary, `libet_tests`, which could be found inside of bin/.