

- Dispatch
- DispatchQueue
-  setSpecific(key:value:) 

Instance Method

# setSpecific(key:value:)

Sets the key/value data for the specified dispatch queue.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
func setSpecific(
    key: DispatchSpecificKey,
    value: T?
) where T : Sendable
```

## Parameters 

`key`  

The key that you use to identify the data.

`value`  

The data you want to associate with the queue.

## See Also

### Getting and Setting Contextual Data

func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with this dispatch queue.

class func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with the current execution context.

class DispatchSpecificKey

A key associated with a specific contextual value on a dispatch queue.

