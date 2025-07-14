

- Dispatch
- DispatchData
- DispatchData.Deallocator
-  DispatchData.Deallocator.custom(\_:\_:) 

Case

# DispatchData.Deallocator.custom(\_:\_:)

Use a custom deallocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
case custom(DispatchQueue?, () -> Void)
```

## See Also

### Deallocators

case free

Use `free` to deallocate memory.

case unmap

Use `munmap` to deallocate memory.

