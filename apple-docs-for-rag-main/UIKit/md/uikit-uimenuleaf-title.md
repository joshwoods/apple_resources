

- UIKit
- UIMenuLeaf
-  title 

Instance Property

# title

A short display title for the menu element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var title: String { get set }
```

**Required**

## See Also

### Managing the appearance

var discoverabilityTitle: String?

A long, informative title to use in the keyboard shortcut overlay.

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

