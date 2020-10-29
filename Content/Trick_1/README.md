# std::map & std::unordered_map & gp_hash_table

Time Complexity:
map > unordered_map > gp_hash_table

map : O(log(n))
unordered_map : O(1)
gp_hash_table : O(1)

Example:
map : 2.406s
unordered_map : 1.042s
gp_hash_table : 0.273s (best)

Usage:
```Cpp
#include <map>

using namespace std;

map <int, int> std_map;

/** Insert **/
std_map[123] = 345;
std_map.insert(make_pair(123, 345));
```


```Cpp
#include <unordered_map>

using namespace std;

map <int, int> std_unordered_map;

/** Insert **/
std_unordered_map[123] = 345;
std_unordered_map.insert(make_pair(123, 345));
```

```Cpp
#include <ext/pb_ds/assoc_container.hpp>

using namespace __gnu_pbds;

gp_hash_table <int, int> hash_table;

/** Insert **/
hash_table[123] = 345;
hash_table.insert(make_pair(123, 345));
```

[link](https://codelearn.io/sharing/hash-table-manh-nhu-the-nao-trong-policy-based-data-structures)
