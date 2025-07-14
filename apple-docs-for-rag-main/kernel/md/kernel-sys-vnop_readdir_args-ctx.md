

- Kernel
- sys
- vnop_readdir_args
-  ctx 

# ctx

Context to authenticate for symlink request.

## See Also

### Fields

If

VNOP_SYMLINK() is successful, the new file should be returned with an iocount which will be dropped by the caller. VFS does not ensure that the target path will have a length shorter than the max symlink length for the filesystem.

dvp

Parent directory for new symlink file.

vpp

cnp

Name information for new symlink.

vap

Attributes for symlink.

target

Path for symlink to store; for "ln -s /var/vardir linktovardir", "target" would be "/var/vardir"

