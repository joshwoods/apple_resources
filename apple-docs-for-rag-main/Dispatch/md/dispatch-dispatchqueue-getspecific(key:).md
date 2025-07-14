

- Dispatch
- DispatchQueue
-  getSpecific(key:) 

Type Method

# getSpecific(key:)

Returns the value for the key associated with the current execution context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
class func getSpecific(key: DispatchSpecificKey) -> T? where T : Sendable
```

## Parameters 

`key`  

The key associated with the dispatch queue.

## See Also

### Getting and Setting Contextual Data

func setSpecific&lt;T>(key: DispatchSpecificKey&lt;T>, value: T?)

Sets the key/value data for the specified dispatch queue.

func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with this dispatch queue.

class DispatchSpecificKey

A key associated with a specific contextual value on a dispatch queue.

