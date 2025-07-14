

- Foundation
- Stream
-  setProperty(\_:forKey:) 

Instance Method

# setProperty(\_:forKey:)

Attempts to set the value of a given property of the receiver and returns a Boolean value that indicates whether the value is accepted by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setProperty(
    _ property: Any?,
    forKey key: Stream.PropertyKey
) -> Bool
```

## Parameters 

`property`  

The value for `key`.

`key`  

The key for one of the receiver’s properties. See Constants for a description of the available property-key constants and expected values.

## Return Value

true if the value is accepted by the receiver, otherwise false.

## See Also

### Configuring Streams

func property(forKey: Stream.PropertyKey) -> Any?

Returns the receiver’s property for a given key.

var delegate: (any StreamDelegate)?

Sets the receiver’s delegate.

