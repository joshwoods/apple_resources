

- Core Foundation
-  CFFileDescriptorDisableCallBacks(\_:\_:) 

Function

# CFFileDescriptorDisableCallBacks(\_:\_:)

Disables callbacks for a given CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorDisableCallBacks(
    _ f: CFFileDescriptor!,
    _ callBackTypes: CFOptionFlags
)
```

## Parameters 

`f`  

A CFFileDescriptor.

`callBackTypes`  

A bitmask that specifies which callbacks to disable (see Callback Identifiers for possible components).

## See Also

### Managing Callbacks

func CFFileDescriptorEnableCallBacks(CFFileDescriptor!, CFOptionFlags)

Enables callbacks for a given CFFileDescriptor.

