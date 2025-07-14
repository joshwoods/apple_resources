

- SwiftUI
- DropInfo
-  itemProviders(for:) Deprecated

Instance Method

# itemProviders(for:)

Returns an array of items that each conform to at least one of the specified uniform type identifiers.

iOS 13.4–18.4DeprecatediPadOS 13.4–18.4DeprecatedMac Catalyst 13.4–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func itemProviders(for types: [String]) -> [NSItemProvider]
```

Deprecated

Use itemProviders(for:) instead.

Show all declarations

## Discussion

This function is only valid during the `performDrop()` action.

## See Also

### Deprecated symbols

func hasItemsConforming(to: [String]) -> Bool

Returns whether at least one item conforms to at least one of the specified uniform type identifiers.

Deprecated

