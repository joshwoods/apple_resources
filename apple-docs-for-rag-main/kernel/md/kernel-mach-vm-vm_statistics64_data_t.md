

- Kernel
- mach
- vm
-  vm_statistics64_data_t 

Structure

# vm_statistics64_data_t

macOS 10.6+

``` source
typedef struct vm_statistics64 {
    ...
} vm_statistics64_data_t;
```

## Topics

### Instance Properties

active_count

compressions

compressor_page_count

cow_faults

decompressions

external_page_count

faults

free_count

hits

inactive_count

internal_page_count

lookups

pageins

pageouts

purgeable_count

purges

reactivations

speculative_count

swapins

swapouts

throttled_count

total_uncompressed_pages_in_compressor

wire_count

zero_fill_count

## See Also

### Statistics

vm_statistics_data_t

vm_extmod_statistics_data_t

vm_purgeable_stat_t

