

- DeviceActivity
- DeviceActivityName
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
extension DeviceActivityName {
    static let bedtime = Self("Bedtime")
}

print(DeviceActivityName.bedtime.rawValue)
// Prints "Bedtime".
```

## See Also

### Creating an Instance

init(rawValue: String)

Creates a new instance with the specified raw value.

init(String)

Creates a new instance with the specified raw value.

