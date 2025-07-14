

- Foundation
- AttributedString
- AttributedString.SingleAttributeTransformer
-  replace(with:value:) 

Instance Method

# replace(with:value:)

Replaces an attribute with a different attribute that a key path identifies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
mutating func replace(
    with keyPath: KeyPath,
    value: U.Value
) where U : AttributedStringKey, U.Value : Sendable
```

## Parameters 

`keyPath`  

The key path that identifies the new attribute.

`value`  

The value of the new attribute.

## See Also

### Replacing Attributes

func replace&lt;U>(with: U.Type, value: U.Value)

Replaces an attribute with a different attribute.

