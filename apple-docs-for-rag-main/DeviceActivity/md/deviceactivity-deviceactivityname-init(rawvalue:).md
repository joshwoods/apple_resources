

- DeviceActivity
- DeviceActivityName
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
extension DeviceActivityName {
    static let bedtime = Self("Bedtime")
}

print(DeviceActivityName.bedtime.rawValue)
// Prints "Bedtime".
```

## See Also

### Creating an Instance

init(String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

