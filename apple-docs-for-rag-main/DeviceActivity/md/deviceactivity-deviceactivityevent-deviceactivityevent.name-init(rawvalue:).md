

- DeviceActivity
- DeviceActivityEvent
- DeviceActivityEvent.Name
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

The raw value to use for the new instance.

## Discussion

The following code example prints the specified raw value.

```
extension DeviceActivityEvent.Name {
    static let event = Self("Event")
}

print(DeviceActivityEvent.Name.event.rawValue)
// Prints "Event".
```

## See Also

### Accessing the Raw Value

init(String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

