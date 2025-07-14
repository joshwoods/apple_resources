

- Kernel
- Kernel Data Types
- scattered_relocation_info
-  r_type 

Instance Property

# r_type

Indicates the type of relocation to be performed. Possible values for this field are shared between this structure and the `relocation_info` data structure; see the description of the `r_type` field in the relocation_info data structure for more details.

macOS 10.8+

``` source
uint32_t r_type:4;
```

