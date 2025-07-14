

- Virtualization
- VZMacOSInstaller
-  install(completionHandler:) 

Instance Method

# install(completionHandler:)

Start installing macOS.

macOS 12.0+

``` source
func install(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

A block the framework calls after installation has completed successfully or has failed.

The `error` parameter passed to the block is `nil` if installation was successful. The framework invokes the block on the VM’s queue. The completion handler returns an `error` parameter that describes the reason for the failure; the `error` is `nil` if installation was successful.

## Discussion

This method starts the installation process. The VM must be in a stopped state. During the installation operation, pausing or stopping the VM results in an undefined behavior.

If you start the installation on the same VZMacOSInstaller object more than once, the framework raises an exception.

Call this method only on the VM’s queue.

## See Also

### Installing macOS

func install() async throws

Start installing macOS.

