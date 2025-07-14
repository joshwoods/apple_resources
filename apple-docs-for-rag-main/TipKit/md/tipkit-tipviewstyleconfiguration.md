

- TipKit
-  TipViewStyleConfiguration 

Structure

# TipViewStyleConfiguration

The container type that holds a tip’s configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct TipViewStyleConfiguration
```

## Topics

### Instance Properties

var actions: [Tips.Action]

var image: Image?

var message: Text?

let tip: any Tip

var title: Text?

## See Also

### View Style

@MainActor @preconcurrency func tipViewStyle(_ style: some TipViewStyle) -> some View 

Sets the given style for TipView within the view hierarchy.

protocol TipViewStyle

A type that applies custom appearance to all tips within a view hierarchy.

struct MiniTipViewStyle

The default style for a TipView.

