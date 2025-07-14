

- AppKit
- NSSearchField
-  rectForSearchText(whenCentered:) Deprecated

Instance Method

# rectForSearchText(whenCentered:)

The rectangle for the search text within the bounds of the field.

macOS 10.11–12.0Deprecated

``` source
@MainActor
func rectForSearchText(whenCentered isCentered: Bool) -> NSRect
```

## Parameters 

`isCentered`  

A Boolean value that indicates whether the search field’s components are centered within the control. For more information, see centersPlaceholder.

## See Also

### Deprecated Symbols

var centersPlaceholder: Bool

A Boolean value that determines whether the search field’s components are centered within the control.

Deprecated

func rectForCancelButton(whenCentered: Bool) -> NSRect

The rectangle for the cancel button within the bounds of the search field.

Deprecated

func rectForSearchButton(whenCentered: Bool) -> NSRect

The rectangle for the search button within the bounds of the search field.

Deprecated

