

- TipKit
-  TipUICollectionViewCell 

Class

# TipUICollectionViewCell

A collection view cell that embeds a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class TipUICollectionViewCell
```

## Overview

Use this cell to create a tip you want to display and layout as a UICollectionViewCell. To configure the content and appearance of your cell, use the configureTip(_:arrowEdge:actionHandler:) function and provide a tip along with an optional arrow edge and action handler. Set the background color of your tip view using backgroundColor.

Adding or removing TipUICollectionViewCell is done by listening to a tip’s shouldDisplayUpdates or statusUpdates.

```
import TipKit
import UIKit

class CatTracksCollectionViewController: UIViewController, UICollectionViewDataSource {
    var collectionView: UICollectionView
    var catTracksFeatureTip = CatTracksFeatureTip()

    override func viewDidLoad() {
        super.viewDidLoad()
        collectionView.register(TipUICollectionViewCell.self, forCellWithReuseIdentifier: "TipUICollectionViewCell")
    }

    override func viewDidAppear(_ animated: Bool) {
        super.viewDidAppear(animated)

        Task { @MainActor in
            for await shouldDisplay in catTracksFeatureTip.shouldDisplayUpdates {
                collectionView.reloadData()
            }
        }
    }

    func collectionView(_ collectionView: UICollectionView, numberOfItemsInSection section: Int) -> Int {
        if section == 0 {
            return catTracksFeatureTip.shouldDisplay ? 1 : 0
        }
        return dataStore.numberOfItemsInSection(section - 1)
    }

    func collectionView(_ collectionView: UICollectionView, cellForItemAt indexPath: IndexPath) -> UICollectionViewCell {
        if let indexPath.section == 0, let catTracksTipCell = collectionView.dequeueReusableCell(withReuseIdentifier: "TipUICollectionViewCell", for: indexPath) as? TipUICollectionViewCell {
            catTracksTipCell.configureTip(catTracksFeatureTip)
            return catTracksTipCell
        }
    }
}
```

## Topics

### Initializers

init?(coder: NSCoder)

init(frame: CGRect)

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

The given style for TipView within the view hierarchy

### Instance Methods

func configureTip(any Tip, arrowEdge: Edge?, actionHandler: (Tips.Action) -> Void) -> Self

Configures the cell to display an embedded tip view.

## Relationships

### Inherits From

- UICollectionViewCell

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

class TipUIView

A user interface element that represents a tip in UIKit applications.

class TipUIPopoverViewController

A view controller that displays a popover tip in UIKit applications.

class TipUICollectionReusableView

A UICollectionReusableView subclass that represents a tip.

