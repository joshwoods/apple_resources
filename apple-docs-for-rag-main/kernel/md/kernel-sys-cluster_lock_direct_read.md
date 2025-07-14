

- Kernel
- sys
-  cluster_lock_direct_read 

Function

# cluster_lock_direct_read

macOS 10.11+

``` source
cl_direct_read_lock_t * cluster_lock_direct_read(vnode_t vp, lck_rw_type_t exclusive);
```

## See Also

### ubc

ubc_blktooff

ubc_create_upl

ubc_getcred

ubc_getsize

ubc_msync

ubc_offtoblk

ubc_page_op

ubc_pages_resident

ubc_range_op

ubc_setsize

ubc_setthreadcred

ubc_upl_abort

ubc_upl_abort_range

ubc_upl_commit

ubc_upl_commit_range

ubc_upl_map

ubc_upl_maxbufsize

ubc_upl_pageinfo

ubc_upl_range_needed

ubc_upl_unmap

cluster_bp

cluster_bp_ext

cluster_copy_ubc_data

cluster_copy_upl_data

cluster_pagein

cluster_pagein_ext

cluster_pageout

cluster_pageout_ext

cluster_push

cluster_push_err

cluster_push_ext

cluster_read

cluster_read_ext

cluster_unlock_direct_read

cluster_update_state

cluster_write

cluster_write_ext

cluster_zero

