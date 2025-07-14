

- Virtualization
- VZMacOSInstaller
-  install() 

Instance Method

# install()

Start installing macOS.

macOS 12.0+

``` source
func install() async throws
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

This method starts the installation process. The VM must be in a stopped state. During the installation operation, pausing or stopping the VM results in an undefined behavior.

If you start the installation on the same VZMacOSInstaller object more than once, the framework raises an exception.

Call this method only on the VM’s queue.

## See Also

### Installing macOS

func install(completionHandler: (Result&lt;Void, any Error>) -> Void)

Start installing macOS.

