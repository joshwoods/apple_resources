

- Core Foundation
-  CFFileDescriptorEnableCallBacks(\_:\_:) 

Function

# CFFileDescriptorEnableCallBacks(\_:\_:)

Enables callbacks for a given CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorEnableCallBacks(
    _ f: CFFileDescriptor!,
    _ callBackTypes: CFOptionFlags
)
```

## Parameters 

`f`  

A CFFileDescriptor.

`callBackTypes`  

A bitmask that specifies which callbacks to enable (see Callback Identifiers for possible components).

## See Also

### Managing Callbacks

func CFFileDescriptorDisableCallBacks(CFFileDescriptor!, CFOptionFlags)

Disables callbacks for a given CFFileDescriptor.

