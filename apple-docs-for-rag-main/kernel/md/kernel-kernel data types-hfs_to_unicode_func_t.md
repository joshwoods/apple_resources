

- Kernel
- Kernel Data Types
-  hfs_to_unicode_func_t 

Type Alias

# hfs_to_unicode_func_t

macOS 10.12+

``` source
typedef int (*hfs_to_unicode_func_t)(const uint8_t hfs_str[32], uint16_t *uni_str, u_int32_t maxCharLen, u_int32_t *usedCharLen);
```

