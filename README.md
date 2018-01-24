PrimeTest executable
====================

This is a simple executable that uses the [Prime](https://github.com/progician/Prime) library which can test a number of being a prime. The executable tests 7 and returns the results: 0 if it passes. It really should pass :)


Building steps
--------------

This project requires the use of conan. It is a basic CMake project otherwise but relies on conan to deliver the Prime library. Here's how:

1. Checkout the repository: `$ git clone https://github.com/progician/PrimeTest.git`
2. Create a build directory: `$ cd PrimeTest && mkdir build && cd build`
3. Get the dependencies: `$ conan install ..`
4. Configure with CMake: `$ cmake .. -GNinja`
5. Build with ninja: `$ ninja`

As long as you have the Prime/1.0.0@progician/test dependency available for conan it will build with no problem and when running it should return with the error code 0. That's all to it.
