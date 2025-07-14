

- Kernel
- mach
- vm
-  vm_statistics_data_t 

Structure

# vm_statistics_data_t

macOS 10.0+

``` source
typedef struct vm_statistics {
    ...
} vm_statistics_data_t;
```

## Topics

### Instance Properties

active_count

cow_faults

faults

free_count

hits

inactive_count

lookups

pageins

pageouts

purgeable_count

purges

reactivations

speculative_count

wire_count

zero_fill_count

## See Also

### Statistics

vm_statistics64_data_t

vm_extmod_statistics_data_t

vm_purgeable_stat_t

