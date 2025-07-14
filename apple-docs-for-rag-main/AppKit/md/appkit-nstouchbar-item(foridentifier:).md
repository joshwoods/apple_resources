

- AppKit
- NSTouchBar
-  item(forIdentifier:) 

Instance Method

# item(forIdentifier:)

Returns the Touch Bar item that corresponds to a given identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
func item(forIdentifier identifier: NSTouchBarItem.Identifier) -> NSTouchBarItem?
```

## Return Value

A Touch Bar item if one exists for the given identifier; otherwise, returns `nil`.

## Discussion

The system returns items (instances of the NSTouchBarItem class) as it finds them, according to the following search order, listed here from first-searched to last-searched:

1.  Items in the bar’s private array, which are reflected in the value of the itemIdentifiers array.

2.  Items in the templateItems array.

3.  Items returned from the bar delegate’s touchBar(_:makeItemForIdentifier:) method.

Your app never needs to instantiate spacing or proxy items because these are created by the system directly, according to their identifiers, as shown in the table below.

| Constant | Resulting item |
|----|----|
| fixedSpaceSmall | small space |
| fixedSpaceLarge | large space |
| flexibleSpace | flexible space |
| otherItemsProxy | proxy placeholder |

For more on the proxy placeholder, see Composition and nesting.

## See Also

### Observing bar status

var isVisible: Bool

A Boolean value that Indicates whether the Touch Bar is eligible for display.

var itemIdentifiers: [NSTouchBarItem.Identifier]

The list of identifiers for the current items in the Touch Bar.

