

- Kernel
- Kernel Functions
-  vn_path_package_check 

Function

# vn_path_package_check

Figure out if a path corresponds to a macOS package.

macOS 10.6+

``` source
int vn_path_package_check(vnode_t vp, char *path, int pathlen, int *component);
```

## Parameters 

`vp`  

Unused.

`path`  

Path to check.

`pathlen`  

Size of path buffer.

`component`  

Set to index of start of last path component if the path is found to be a package. Set to -1 if the path is not a known package type.

## Return Value

0 unless some parameter was invalid, in which case EINVAL is returned. Determine package-ness by checking what \*component is set to.

## Discussion

Determines if the extension on a path is a known macOS extension type.

