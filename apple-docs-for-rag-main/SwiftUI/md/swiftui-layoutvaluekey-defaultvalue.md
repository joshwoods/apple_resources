

- SwiftUI
- LayoutValueKey
-  defaultValue 

Type Property

# defaultValue

The default value of the key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var defaultValue: Self.Value { get }
```

**Required**

## Discussion

Implement the `defaultValue` property for a type that conforms to the LayoutValueKey protocol. For example, you can create a `Flexibility` layout value that defaults to `nil`:

```
private struct Flexibility: LayoutValueKey {
    static let defaultValue: CGFloat? = nil
}
```

The type that you declare for the `defaultValue` sets the layout key’s Value associated type. The Swift compiler infers the key’s associated type in the above example as an optional CGFloat.

Any view that you don’t explicitly set a value for uses the default value. Override the default value for a view using the layoutValue(key:value:) modifier.

## See Also

### Providing a default value

associatedtype Value

The type of the key’s value.

**Required**

