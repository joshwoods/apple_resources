

- AppKit
- NSSearchField
-  centersPlaceholder Deprecated

Instance Property

# centersPlaceholder

A Boolean value that determines whether the search field’s components are centered within the control.

macOS 10.11–12.0Deprecated

``` source
@MainActor
var centersPlaceholder: Bool { get set }
```

Deprecated

The placeholder centering UI design is no longer available. Setting this property is no-op.

## Discussion

When this property is set to true, the search field’s components become centered within the control if the field is empty and doesn’t have focus. If the field is empty when receiving focus, the centered objects animate to the edges of the control. When this property is set to false, the components are always at the edge. The default value is true.

Note

When set to true, wantsLayer is also true.

## See Also

### Deprecated Symbols

func rectForCancelButton(whenCentered: Bool) -> NSRect

The rectangle for the cancel button within the bounds of the search field.

Deprecated

func rectForSearchButton(whenCentered: Bool) -> NSRect

The rectangle for the search button within the bounds of the search field.

Deprecated

func rectForSearchText(whenCentered: Bool) -> NSRect

The rectangle for the search text within the bounds of the field.

Deprecated

