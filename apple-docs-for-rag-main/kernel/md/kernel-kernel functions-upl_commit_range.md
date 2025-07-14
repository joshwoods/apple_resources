

- Kernel
- Kernel Functions
-  upl_commit_range 

Function

# upl_commit_range

macOS 10.1+

``` source
kern_return_t upl_commit_range(upl_t upl_object, upl_offset_t offset, upl_size_t size, integer_t cntrl_flags, upl_page_info_array_t page_list, mach_msg_type_number_t page_listCnt, boolean_t *empty);
```

