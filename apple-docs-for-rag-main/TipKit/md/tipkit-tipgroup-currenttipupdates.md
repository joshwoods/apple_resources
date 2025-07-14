

- TipKit
- TipGroup
-  currentTipUpdates 

Instance Property

# currentTipUpdates

Stream of tips that become eligible for display.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final var currentTipUpdates: some AsyncSequence { get }
```

## See Also

### Getting the currently available tip

var currentTip: (any Tip)?

Returns the current tip available for display.

