

- UIKit
- UITextItem
-  UITextItem.Content 

Enumeration

# UITextItem.Content

Constants that describe and capture the type of content a text item represents along with a specific related value.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
enum Content
```

## Topics

### Getting the content type

case link(URL)

A link to a resource, such as an item on a remote server or the path to a local file.

case tag(String)

A string that represents a custom tag for a topic.

case textAttachment(NSTextAttachment)

A text attachment, such as an image or view.

## See Also

### Specifying the content type

var content: UITextItem.Content

The content type and related value of the text item.

