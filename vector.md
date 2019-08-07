```cpp
//std::vector::emplace_back 
//Construct and insert element at the end
//Inserts a new element at the end of the vector, right after its current last element. This new element is constructed in place using args as the arguments for its constructor.

// vector::emplace_back
#include <iostream>
#include <vector>

int main ()
{
  std::vector<int> myvector = {10,20,30};

  myvector.emplace_back (100);
  myvector.emplace_back (200);

  std::cout << "myvector contains:";
  for (auto& x: myvector)
    std::cout << ' ' << x;
  std::cout << '\n';

  return 0;
}
```

