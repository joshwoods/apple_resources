

- UIKit
- Drag and drop
-  Understanding a drag item as a promise 

Article

# Understanding a drag item as a promise

Use drag items to convey data representation promises between a source app and a destination app.

iOS 11.0+iPadOS 11.0+

## Overview

When a user drags an onscreen visual representation of an item in your app, such as a photo, a Maps location, a Calendar event, or a text selection, your app associates the underlying data with a *drag item*. The drag item, in turn, uses an *item provider*. Your app populates the item provider’s registeredTypeIdentifiers array with uniform type identifiers (UTIs).

The array of UTIs constitutes the source app’s promise about the specific data representations it can deliver, on request, to a destination app. The term *promise* means that, at the time your app constructs a drag item, it commits to providing certain data representations but doesn’t yet perform the work to create them. Although it appears to the user that the item itself is being dragged, the drag item instead consists of promises along with a preview image that remains under the user’s touch point onscreen.

The portion of your app that constructs the drag item is the *drag interaction delegate* (UIDragInteractionDelegate). On the destination side, an app’s *drop interaction delegate* (UIDropInteractionDelegate) interacts with the drag item to consume promised data.

This table shows the protocols you implement to support constructing or consuming a drag item, depending on whether a view in your app is acting as a source or destination:

| Drag-and-drop role | Protocol | Your implementation |
|----|----|----|
| Source app | NSItemProviderWriting | Register UTIs |
| Destination app | NSItemProviderReading | Request items |

The following classes automatically support these protocols: NSString, NSAttributedString, NSURL, UIColor, and UIImage.

## See Also

### Essentials

Making a view into a drag source

Adopt drag interaction APIs to provide items for dragging.

Making a view into a drop destination

Adopt drop interaction APIs to selectively consume dragged content.

Adopting drag and drop in a custom view

Demonstrates how to enable drag and drop for a `UIImageView` instance.

Adopting drag and drop in a table view

Demonstrates how to enable and implement drag and drop for a table view.

