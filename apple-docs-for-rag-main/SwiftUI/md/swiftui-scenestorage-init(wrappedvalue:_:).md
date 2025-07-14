

- SwiftUI
- SceneStorage
-  init(wrappedValue:\_:) 

Initializer

# init(wrappedValue:\_:)

Creates a property that can save and restore an integer, transforming it to a `RawRepresentable` data type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    wrappedValue: Value,
    _ key: String
) where Value : RawRepresentable, Value.RawValue == Int
```

Show all declarations

## Parameters 

`wrappedValue`  

The default value if an integer value is not available for the given key.

`key`  

A key used to save and restore the value.

## Discussion

A common usage is with enumerations:

```
enum MyEnum: Int {
    case a
    case b
    case c
}
struct MyView: View {
    @SceneStorage("MyEnumValue") private var value = MyEnum.a
    var body: some View { ... }
}
```

## See Also

### Storing a value

init(_:)

Creates a property that can save and restore an Optional boolean.

