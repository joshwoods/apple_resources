

- Core Foundation
-  CFAllocatorGetDefault() 

Function

# CFAllocatorGetDefault()

Gets the default allocator object for the current thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorGetDefault() -> Unmanaged!
```

## Return Value

A reference to the default allocator for the current thread. If none has been explicitly set, returns the generic system allocator, kCFAllocatorSystemDefault. Ownership follows The Get Rule.

## Discussion

See the discussion for CFAllocatorSetDefault(_:) for more detail on the default allocator and for advice on how and when to set a custom allocator as the default.

## See Also

### Getting and Setting the Default Allocator

func CFAllocatorSetDefault(CFAllocator!)

Sets the given allocator as the default for the current thread.

