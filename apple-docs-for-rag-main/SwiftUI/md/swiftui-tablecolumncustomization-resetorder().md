

- SwiftUI
- TableColumnCustomization
-  resetOrder() 

Instance Method

# resetOrder()

Resets the column order back to the default, preserving the customized visibility and size.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
mutating func resetOrder()
```

## Discussion

Tables that are bound to this state will order their columns as described by their column builder.

## See Also

### Managing the customization

subscript(visibility _: String) -> Visibility

The visibility of the column identified by its identifier.

