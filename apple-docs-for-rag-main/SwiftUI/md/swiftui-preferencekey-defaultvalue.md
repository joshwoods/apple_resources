

- SwiftUI
- PreferenceKey
-  defaultValue 

Type Property

# defaultValue

The default value of the preference.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var defaultValue: Self.Value { get }
```

**Required** Default implementation provided.

## Discussion

Views that have no explicit value for the key produce this default value. Combining child views may remove an implicit value produced by using the default. This means that `reduce(value: &x, nextValue: {defaultValue})` shouldn’t change the meaning of `x`.

## Default Implementations

### PreferenceKey Implementations

static var defaultValue: Self.Value

Let nil-expressible values default-initialize to nil.

## See Also

### Getting the default value

associatedtype Value

The type of value produced by this preference.

**Required**

