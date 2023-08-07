# GoogleTest for Unikraft

This is the port of [GoogleTest](https://google.github.io/googletest/) to Unikraft.

Some libraries that use GoogleTest rely on it to also provide a boilerplate main function to run their tests.
Providing this function by default might however conflict with the application's intended main.
For this purpose the LIBGOOGLETEST_BUILD_MAIN config option controls whether GoogleTest provides a `main()` function.
								 
GoogleTest being a C++ library, `libcxx` is required.
`lib-googletest` should come at the end of the dependency list.

Please refer to `README.md` in the main unikraft repository as well as the [Unikraft Homepage](https://unikraft.org/) for further information.
