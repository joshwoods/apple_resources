

- TipKit
-  TipUIView 

Class

# TipUIView

A user interface element that represents a tip in UIKit applications.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class TipUIView
```

## Overview

Use this view to create a tip you want to display and lay out as a UIView. To configure the content and appearance of your view, use the init(_:arrowEdge:actionHandler:) function and provide a tip along with an optional arrow edge and optional action. Set the background color of your tip view using backgroundColor.

Adding and removing TipUIView from your app is done by listening to a tip’s shouldDisplayUpdates or statusUpdates.

```
import TipKit
import UIKit

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

class CatTracksViewController: UIViewController {
    private var catTracksFeatureTip = CatTracksFeatureTip()
    private var tipObservationTask: Task?
    private weak var tipView: TipUIView?    

    override func viewDidAppear(_ animated: Bool) {
        super.viewDidAppear(animated)

        tipObservationTask = tipObservationTask ?? Task { @MainActor in
            for await shouldDisplay in catTracksFeatureTip.shouldDisplayUpdates {
                if shouldDisplay {
                    let tipHostingView = TipUIView(catTracksFeatureTip)
                    tipHostingView.translatesAutoresizingMaskIntoConstraints = false

                    view.addSubview(tipHostingView)

                    view.addConstraints([
                        tipHostingView.centerYAnchor.constraint(equalTo: view.centerYAnchor),
                        tipHostingView.leadingAnchor.constraint(equalTo: view.leadingAnchor, constant: 20.0),
                        tipHostingView.trailingAnchor.constraint(equalTo: view.trailingAnchor, constant: -20.0)
                    ])

                    tipView = tipHostingView
                }
                else {
                    tipView?.removeFromSuperview()
                    tipView = nil
                }
            }
        }
    }
}

override func viewWillDisappear(_ animated: Bool) {
    super.viewWillDisappear(animated)

    tipObservationTask?.cancel()
    tipObservationTask = nil
}
```

## Topics

### Initializers

init(any Tip, arrowEdge: Edge?, actionHandler: (Tips.Action) -> Void)

Creates a tip view with an optional arrow edge and action handler.

### Instance Properties

var backgroundColor: UIColor?

The background color to use for the tip view.

var cornerRadius: CGFloat

Corner radius for the tip view.

var imageSize: CGSize

Size of the image displayed in the tip view.

var imageStyle: (any ShapeStyle)?

Foreground style for the tip’s image.

var viewStyle: any TipViewStyle

The given style for TipView within the view hierarchy.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### UIKit Views

class TipUIPopoverViewController

A view controller that displays a popover tip in UIKit applications.

class TipUICollectionViewCell

A collection view cell that embeds a tip.

class TipUICollectionReusableView

A UICollectionReusableView subclass that represents a tip.

