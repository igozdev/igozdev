```cpp
// main.cpp
#include <iostream>
#include <limits>

auto main([[maybe_unused]] int argc, [[maybe_unused]] char** argv) -> int {
    std::operator<<(std::cout, "Hello, world!").operator<<(std::endl);
    constexpr auto int_min = std::numeric_limits<int>::min();
    return int_min % -((int)sizeof(+char{})["Goodbye, world."]);
            // ISO/IEC JTC1/SC22/WG21 4842:2024, [expr.mul]
            //     "... if the quotient a/b is representable in the type
            //      of the result, (a/b)*b + a%b is equal to a; otherwise,
            //      the behavior of both a/b and a%b is undefined."
}
```
