

- TipKit
-  TipUIPopoverViewController 

Class

# TipUIPopoverViewController

A view controller that displays a popover tip in UIKit applications.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class TipUIPopoverViewController
```

## Overview

Use this view controller to present a tip you want to display using UIPopoverPresentationController.

Presenting or dismissing TipUIPopoverViewController is done by listening to a tip’s shouldDisplayUpdates or statusUpdates.

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
    @IBOutlet weak var catTracksFeatureButton: UIButton!

    private var catTracksFeatureTip = CatTracksFeatureTip()
    private var tipObservationTask: Task?
    private weak var tipPopoverController: TipUIPopoverViewController?

    override func viewDidAppear(_ animated: Bool) {
        super.viewDidAppear(animated)

        tipObservationTask = tipObservationTask ?? Task { @MainActor in
            for await shouldDisplay in catTracksFeatureTip.shouldDisplayUpdates {
                if shouldDisplay {
                    let popoverController = TipUIPopoverViewController(catTracksFeatureTip, sourceItem: catTracksFeatureButton)
                    present(popoverController, animated: animated)
                    tipPopoverController = popoverController
                }
                else {
                    if presentedViewController is TipUIPopoverViewController {
                        dismiss(animated: animated)
                        tipPopoverController = nil
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
}
```

## Topics

### Initializers

convenience init(any Tip, sourceItem: any UIPopoverPresentationControllerSourceItem, actionHandler: (Tips.Action) -> Void)

Initializes a popover controller with the specified tip.

init?(coder: NSCoder)

init(nibName: String?, bundle: Bundle?)

### Instance Properties

var backgroundColor: UIColor?

The background color to use for the tip view.

var imageSize: CGSize

Size of the image displayed in the tip view.

var imageStyle: (any ShapeStyle)?

Foreground style for the tip’s image.

var presentationDelegate: (any UIPopoverPresentationControllerDelegate)?

The popover presentation delegate, which lets you customize the behavior of a popover-based presentation.

var sourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item on which to anchor the tip popover.

var viewStyle: any TipViewStyle

The given style for TipView within the view hierarchy.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### UIKit Views

class TipUIView

A user interface element that represents a tip in UIKit applications.

class TipUICollectionViewCell

A collection view cell that embeds a tip.

class TipUICollectionReusableView

A UICollectionReusableView subclass that represents a tip.

