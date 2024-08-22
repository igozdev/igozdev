```cpp
// main.cpp
#include <iostream>

auto main([[maybe_unused]] int argc, [[maybe_unused]] char** argv) -> int {
    std::operator<<(std::cout, "Hello, world!").operator<<(std::endl);
    return 0;
}
```
