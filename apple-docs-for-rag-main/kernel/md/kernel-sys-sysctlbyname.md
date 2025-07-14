

- Kernel
- sys
-  sysctlbyname 

Function

# sysctlbyname

Gets or sets information about the system and environment.

macOS 10.0+

``` source
int sysctlbyname(const char *, void *, size_t *, void *, size_t);
```

## Parameters 

`name`  

The ASCII name of the requested attribute. To obtain a list of attribute names for the current system, run `sysctl -a` from Terminal.

`oldp`  

A pointer to a buffer that receives the requested data. Specify the size of this buffer using the `oldlenp` parameter. The function copies the requested data into this buffer as space allows. If the buffer is too small to hold all the data, the function updates the `oldlenp` parameter with the required size.

Specify `NULL` if you don’t want to get the attribute’s value. For example, set this parameter to `NULL` and specify a valid parameter in `oldlenp` to get the size of the data.

`oldlenp`  

A variable that contains the number of bytes in the buffer in the `oldp` parameter. If the amount of data is greater than the value in this parameter, the function updates this parameter to the required size and returns `ENOMEM`. (The function doesn’t modify the value if it’s larger than or equal to the amount of available data).

Specify `NULL` if you don’t want to get the attribute’s value.

`newp`  

A pointer to a buffer that contains new data to assign to the attribute. The function copies the data from this buffer to the attribute. You must specify the size of this buffer using the `newlen` parameter. Specify `NULL` if you don’t want to set the attribute’s value.

A process must have the root-level privileges to set system information.

`newlen`  

A variable that contains the size of the buffer in the `newp` parameter, in bytes. Specify `0` if you don’t want to set the attribute’s value.

## Return Value

0 on success, or an error code that indicates a problem occurred. Possible error codes include `EFAULT`, `EINVAL`, `ENOMEM`, `ENOTDIR`, `EISDIR`, `ENOENT`, and `EPERM`.

## Discussion

This function offers a programmatic alternative to the sysctl command-line tool. Use it to get or set relevant system information, and to make decisions dynamically based on the current system information. For example, you might use the `hw.cachelinesize` attribute to align data in your data structures. Making decisions dynamically is especially important for universal binaries that run on Apple silicon or Intel-based Mac computers.

The following example shows how to retrieve the cache line size using this function.

int64_t cacheLineSize() {
    int64_t ret = 0;
    size_t size = sizeof(ret);

    if (sysctlbyname(&quot;hw.cachelinesize&quot;, &amp;ret, &amp;size, NULL, 0) == -1) {
        NSLog(@&quot;cacheLineSize failed with error: %d&quot;, errno);

        return -1;
    }

    return ret;
}

## Topics

### Parameters

Determining system capabilities

Interrogate the system for processor, cache, and topology information.

Determining Instruction Set Characteristics

Interrogate the system for details about the instruction set.

## See Also

### sysctl

sysctl_handle_int

sysctl_handle_int2quad

sysctl_handle_long

sysctl_handle_opaque

sysctl_handle_quad

sysctl_handle_string

sysctl_io_number

sysctl_io_opaque

sysctl_io_string

sysctl_register_oid

sysctl_unregister_oid

sysctl__children

sysctl__debug_children

sysctl__hw_children

sysctl__kern_children

sysctl__machdep_children

sysctl__net_children

sysctl__sysctl_children

sysctl__user_children

sysctl__vfs_children

sysctl__vm_children

