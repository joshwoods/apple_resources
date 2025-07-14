

- TipKit
-  TipNSPopover 

Class

# TipNSPopover

A subclass of NSPopover that displays a popover tip in AppKit applications.

macOS 14.0+

``` source
@MainActor @objc @preconcurrency
final class TipNSPopover
```

## Overview

Use this to create a tip you want to display and lay out as a NSPopover.

Adding and removing TipNSView from your app is done by listening to a tip’s shouldDisplayUpdates or statusUpdates.

```
import Cocoa
import TipKit

struct CatTracksFeatureTip: Tip {
    var title: Text {
        Text("Sample tip title")
    }

    var message: Text? {
        Text("Sample tip message")
    }

    var image: Image? {
        Image(systemName: "globe")
    }
}

class CatTracksViewController: NSViewController {
    @IBOutlet weak var catTracksFeatureButton: NSButton!

    private var catTracksFeatureTip = CatTracksFeatureTip()
    private var tipObservationTask: Task?
    private var tipPopover: TipNSPopover?

    override func viewDidAppear() {
        super.viewDidAppear()

        tipObservationTask = tipObservationTask ?? Task { @MainActor in
            for await shouldDisplay in catTracksFeatureTip.shouldDisplayUpdates {
                if shouldDisplay {
                    tipPopover = TipNSPopover(catTracksFeatureTip)
                    tipPopover?.show(relativeTo: catTracksFeatureButton.bounds, of: catTracksFeatureButton, preferredEdge: .minY)
                }
                else {
                    tipPopover?.close()
                    tipPopover = nil
                }
            }
        }
    }

    override func viewDidDisappear() {
        super.viewDidDisappear()

        tipObservationTask?.cancel()
        tipObservationTask = nil
    }
}
```

## Topics

### Initializers

init(any Tip, delegate: (any NSPopoverDelegate)?, actionHandler: (Tips.Action) -> Void)

Initializes a popover with the specified tip.

### Instance Properties

var backgroundColor: NSColor?

The background color to use for the tip view.

var cornerRadius: CGFloat

Corner radius for the tip view.

var imageSize: CGSize

Size of the image displayed in the tip view.

var imageStyle: (any ShapeStyle)?

Foreground style for the tip’s image.

var viewStyle: any TipViewStyle

The given style for TipView within the view hierarchy

## Relationships

### Inherits From

- NSPopover

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAppearanceCustomization
- NSCoding
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring

## See Also

### AppKit Views

class TipNSView

A user interface element that represents a tip in AppKit applications.

