

- System Configuration
- SCPreferencesContext
-  init(version:info:retain:release:copyDescription:) 

Initializer

# init(version:info:retain:release:copyDescription:)

Creates a preferences context with the specified raw values.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer?,
    retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?,
    release: ((UnsafeRawPointer) -> Void)?,
    copyDescription: ((UnsafeRawPointer) -> Unmanaged)?
)
```

