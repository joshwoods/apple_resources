

- AppKit
-  NSPreviewRepresentingActivityItem 

Class

# NSPreviewRepresentingActivityItem

A type that adds metadata to an item you share using the macOS share sheet.

macOS 13.0+

``` source
class NSPreviewRepresentingActivityItem
```

## Overview

An NSPreviewRepresentingActivityItem object provides a concrete implementation of the NSPreviewRepresentableActivityItem protocol. Use it to create shareable items for common types such as strings or images, or when you don’t want to adopt the NSPreviewRepresentableActivityItem protocol directly in your app’s objects. To share the item from your app, initialize the NSSharingServicePicker object with this object.

Note

If your data consists of a URL, pass that URL directly to the sharing service picker instead of using this class.

## Topics

### Creating a Preview Activity Item

convenience init(item: Any, title: String?, image: NSImage?, icon: NSImage?)

Creates a metadata object with the title, image, and icon for a shareable item.

init(item: Any, title: String?, imageProvider: NSItemProvider?, iconProvider: NSItemProvider?)

Creates a metadata object that provides a title and images for a shareable item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSPreviewRepresentableActivityItem

## See Also

### Share Panel

class NSSharingServicePicker

A list of sharing services that the user can choose from.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

