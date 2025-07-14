

- Kernel
- Kernel Structures
-  libsptm_state_t 

Structure

# libsptm_state_t

macOS 15.4+

``` source
typedef struct sptm_client_state {
    ...
} libsptm_state_t;
```

## Topics

### Instance Properties

cpu_features

feature_flags

first_papt

first_phys

frame_table

frame_type_params

io_frame_table

last_papt

last_phys

max_cpus

n_io_ranges

n_papt_ranges

papt_ranges

percpu_dispatch_state

percpu_xnu_saved_state

pt_attr_table

reserved

root_table_paddr

sptm_first_tag_storage_paddr

sptm_last_tag_storage_paddr

sptm_panicking_cpu_id

trace_buffer

version

