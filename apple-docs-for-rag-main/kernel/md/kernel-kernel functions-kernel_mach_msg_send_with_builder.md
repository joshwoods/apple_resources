

- Kernel
- Kernel Functions
-  kernel_mach_msg_send_with_builder 

Function

# kernel_mach_msg_send_with_builder

macOS 13.1+

``` source
mach_msg_return_t kernel_mach_msg_send_with_builder(mach_msg_size_t descriptor_count, mach_msg_size_t payload_size, void (^builder)(mach_msg_header_t *header, mach_msg_descriptor_t *descs, void *payload));
```

