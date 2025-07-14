

- Kernel
- Kernel Functions
-  vn_rdwr_64 

Function

# vn_rdwr_64

macOS 15.0+

``` source
int vn_rdwr_64(enum uio_rw rw, struct vnode *vp, uint64_t base, int64_t len, off_t offset, enum uio_seg segflg, int ioflg, kauth_cred_t cred, int64_t *aresid, struct proc *p);
```

