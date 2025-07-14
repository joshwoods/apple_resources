

- Kernel
- sys
-  cdevsw_add_with_bdev 

Function

# cdevsw_add_with_bdev

macOS 10.4+

``` source
int cdevsw_add_with_bdev(int index, const struct cdevsw *csw, int bdev);
```

## See Also

### Block Device

bdevsw_add

bdevsw_isfree

bdevsw_remove

cdevsw_add

cdevsw_isfree

cdevsw_remove

