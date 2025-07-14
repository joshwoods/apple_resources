

- Kernel
- Kernel Functions
-  vn_getpath 

Function

# vn_getpath

Construct the path to a vnode.

macOS 10.4+

``` source
int vn_getpath(struct vnode *vp, char *pathbuf, int *len);
```

## Parameters 

`vp`  

The vnode whose path to obtain.

`pathbuf`  

Destination for pathname; should be of size MAXPATHLEN

`len`  

Destination for length of resulting path string. Result will include NULL-terminator in count--that is, "len" will be strlen(pathbuf) + 1.

## Return Value

0 for success or an error code.

## Discussion

Paths to vnodes are not always straightforward: a file with multiple hard-links will have multiple pathnames, and it is sometimes impossible to determine a vnode's full path. vn_getpath() will not enter the filesystem.

