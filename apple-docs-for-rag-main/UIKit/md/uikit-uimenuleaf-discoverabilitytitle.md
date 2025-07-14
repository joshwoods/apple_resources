

- UIKit
- UIMenuLeaf
-  discoverabilityTitle 

Instance Property

# discoverabilityTitle

A long, informative title to use in the keyboard shortcut overlay.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var discoverabilityTitle: String? { get set }
```

**Required**

## See Also

### Managing the appearance

var title: String

A short display title for the menu element.

**Required**

var image: UIImage?

An image that appears next to the menu element.

**Required**

var attributes: UIMenuElement.Attributes

The attributes that determine the style of the menu element.

**Required**

var presentationSourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item you can use as an anchor for subsequent presentations.

**Required**

