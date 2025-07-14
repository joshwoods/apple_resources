

- AppKit
- NSTouchBar
-  isVisible 

Instance Property

# isVisible

A Boolean value that Indicates whether the Touch Bar is eligible for display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var isVisible: Bool { get }
```

## Discussion

A value of true indicates that the bar is attached to an eligible bar provider and that its items are displayable, assuming adequate geometric space. A *bar provider* is an object that conforms to the NSTouchBarProvider protocol. For more on bar providers, read Bar objects.

This property is key–value observable.

## See Also

### Observing bar status

var itemIdentifiers: [NSTouchBarItem.Identifier]

The list of identifiers for the current items in the Touch Bar.

func item(forIdentifier: NSTouchBarItem.Identifier) -> NSTouchBarItem?

Returns the Touch Bar item that corresponds to a given identifier.

