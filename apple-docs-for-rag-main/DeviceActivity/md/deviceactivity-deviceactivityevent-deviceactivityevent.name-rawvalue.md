

- DeviceActivity
- DeviceActivityEvent
- DeviceActivityEvent.Name
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var rawValue: String
```

## Discussion

A new instance initialized with `rawValue` prints the specified raw value. For example:

```
extension DeviceActivityEvent.Name {
    static let event = Self("Event")
}

print(DeviceActivityEvent.Name.event.rawValue)
// Prints "Event".
```

## See Also

### Accessing the Raw Value

init(rawValue: String)

Creates a new instance with the specified raw value.

init(String)

Creates a new instance with the specified raw value.

