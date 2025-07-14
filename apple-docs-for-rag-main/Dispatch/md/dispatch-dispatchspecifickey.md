

- Dispatch
-  DispatchSpecificKey 

Class

# DispatchSpecificKey

A key associated with a specific contextual value on a dispatch queue.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
final class DispatchSpecificKey
```

## Overview

Access the value of a key using the setSpecific(key:value:) and getSpecific(key:) methods.

## Topics

### Creating a Key

init()

## Relationships

### Conforms To

- Sendable

## See Also

### Getting and Setting Contextual Data

func setSpecific&lt;T>(key: DispatchSpecificKey&lt;T>, value: T?)

Sets the key/value data for the specified dispatch queue.

func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with this dispatch queue.

class func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with the current execution context.

