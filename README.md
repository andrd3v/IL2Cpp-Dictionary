# IL2Cpp-Dictionary external
IL2CPP Dictionary and monoArray

# Usage 
```c++
using players_dict = Dictionary<int, mach_vm_address_t>;
mach_vm_address_t players_dict_obj_addr = Read<mach_vm_address_t>(inst + 0x28, so2_task);

players_dict dict(so2_task, (uintptr_t)players_dict_obj_addr);
int count = dict.get_Count();

auto keys = dict.get_Keys();
auto values = dict.get_Values();
```

# Credits
- [andrd3v](https://github.com/andrd3v)
