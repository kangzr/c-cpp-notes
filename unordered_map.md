```cpp
// std::unordered_map::emplace
// Construct and insert element
// Inserts a new element in the unordered_map if its key is unique. This new element is constructed in place using args as the arguments for the element's constructor.
// unordered_map::emplace

#include <iostream>
#include <string>
#include <unordered_map>

int main ()
{
  std::unordered_map<std::string,std::string> mymap;

  mymap.emplace ("NCC-1701", "J.T. Kirk");
  mymap.emplace ("NCC-1701-D", "J.L. Picard");
  mymap.emplace ("NCC-74656", "K. Janeway");

  std::cout << "mymap contains:" << std::endl;
  for (auto& x: mymap)
    std::cout << x.first << ": " << x.second << std::endl;

  std::cout << std::endl;
  return 0;
}
```

