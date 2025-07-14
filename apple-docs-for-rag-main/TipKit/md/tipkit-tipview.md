

- TipKit
-  TipView 

Structure

# TipView

A user interface element that represents an inline tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct TipView where Content : Tip
```

## Overview

You create a tip view by providing a tip along with an optional arrow edge and action handler. The tip is a type that conforms to the Tip protocol. The arrow edge is a directional arrow pointing away from the tip. The action is a closure that executes when the user triggers a tip’s button.

For example, display a tip view, above an image, with an arrow edge along the bottom:

1.  Define your tip’s content as a structure conforming to the `Tip` protocol.

2.  Create an instance your tip as a variable in the view containing the feature you want to highlight.

3.  Create an instance of a `TipView`, near the feature you want to highlight, passing in the instance your tip’s content, along with an optional arrow edge.

4.  Then configure and load the tips for your app by calling configure(_:).

Important

Use TipUIView and TipNSView when adding tips to UIView and NSView hierarchies.

```
import SwiftUI
import TipKit

// Define your tip's content.
struct SampleTip: Tip {
    var title: Text {
        Text("Save as a Favorite")
    }

    var message: Text? {
        Text("Your favorite backyards always appear at the top of the list.")
    }

    var image: Image? {
        Image(systemName: "star")
    }
}

struct SampleView: View {
    // Create an instance of your tip.
    var tip = SampleTip()

    var body: some View {
        VStack {
            // Place the tip view near the feature you want to highlight.
            // Tips.configure(options:) must be called before your tip will be eligible for display.
            TipView(tip, arrowEdge: .bottom)
        }
    }
}
```

## Topics

### Creating a tip view

init((any Tip)?, arrowEdge: Edge?, action: (Tips.Action) -> Void)

Creates a tip view with an optional arrow.

### Initializers

init(Content, arrowEdge: Edge?, action: (Tips.Action) -> Void)

Creates a tip view with an optional arrow.

## Relationships

### Conforms To

- View

## See Also

### Views

@MainActor @preconcurrency func popoverTip(_ tip: (any Tip)?, arrowEdge: Edge? = nil, action: @escaping (Tips.Action) -> Void = { _ in }) -> some View 

Presents a popover tip on the modified view.

