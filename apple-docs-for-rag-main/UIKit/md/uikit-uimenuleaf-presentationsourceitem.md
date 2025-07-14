

- UIKit
- UIMenuLeaf
-  presentationSourceItem 

Instance Property

# presentationSourceItem

The item you can use as an anchor for subsequent presentations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var presentationSourceItem: (any UIPopoverPresentationControllerSourceItem)? { get }
```

**Required**

## Discussion

The system populates this property during the execution of the menu element’s action (its handler or selector). For example, for a menu element in a menu that presents from a UIButton, the system may populate this property with that button.

Use this property to specify where to anchor popovers when a person taps the menu element, like in the following code.

```
let share = UIAction(title: "Share") { [unowned self] action in
    let shareVC = UIActivityViewController(activityItems: items, applicationActivities: activities)
    shareVC.modalPresentationStyle = .popover
    shareVC.popoverPresentationController?.sourceItem = action.presentationSourceItem
    present(shareVC, animated: true)
}
```

## See Also

### Managing the appearance

var title: String

A short display title for the menu element.

**Required**

var discoverabilityTitle: String?

A long, informative title to use in the keyboard shortcut overlay.

**Required**

var image: UIImage?

An image that appears next to the menu element.

**Required**

var attributes: UIMenuElement.Attributes

The attributes that determine the style of the menu element.

**Required**

