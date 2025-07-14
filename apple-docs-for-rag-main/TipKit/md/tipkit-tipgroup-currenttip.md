

- TipKit
- TipGroup
-  currentTip 

Instance Property

# currentTip

Returns the current tip available for display.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor
final var currentTip: (any Tip)? { get }
```

## See Also

### Getting the currently available tip

var currentTipUpdates: some AsyncSequence&lt;any Tip, Never>

Stream of tips that become eligible for display.

