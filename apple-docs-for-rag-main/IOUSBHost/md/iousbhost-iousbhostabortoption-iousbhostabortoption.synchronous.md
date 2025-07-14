

- IOUSBHost
- IOUSBHostAbortOption
-  IOUSBHostAbortOption.synchronous 

Case

# IOUSBHostAbortOption.synchronous

The option to abort input/output requests synchronously.

Mac Catalyst 14.0+macOS 10.15+

``` source
case synchronous
```

## Discussion

This is the default argument for functions that abort pending input/output requests. All input/output requests must abort before functions can return.

## See Also

### Options

case asynchronous

The option to abort input/output requests asynchronously.

