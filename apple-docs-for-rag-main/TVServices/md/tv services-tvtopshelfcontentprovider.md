

- TV Services
-  TVTopShelfContentProvider 

Class

# TVTopShelfContentProvider

The main interface for your Top Shelf app extension, which you use to provide content for the top shelf area of the tvOS Home Screen.

tvOS 13.0+

``` source
class TVTopShelfContentProvider
```

## Overview

Adopt this protocol in the principal class of your Top Shelf app extension. Use its methods to create the items that you want to display in the top shelf interface. For each item, specify additional resources such as the image or video to display.

Fill the top shelf area with the user’s active content or with content you want to highlight or promote. For each distinct piece of content, create a TVTopShelfCarouselItem or TVTopShelfSectionedItem and fill the object with details about that content. For example, provide an identifier for the item and URLs for the pictures or videos you want to display for that item. After creating your items, add them to an appropriate content object and return them from your loadTopShelfContent(completionHandler:) method.

## Topics

### Providing the Top Shelf Content

func loadTopShelfContent(completionHandler: ((any TVTopShelfContent)?) -> Void)

Provides the content you want to display in the top shelf for your app.

### Updating Your Content

class func topShelfContentDidChange()

Tells the system that your top shelf content changed and requires an update.

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

## See Also

### Top shelf app extensions

Building a Full Screen Top Shelf Extension

Highlight content from your Apple TV application by building a full screen Top Shelf extension.

Legacy Extension

Help users discover your app by providing top shelf content and a description of your tvOS app.

