

- Foundation
-  NSExtensionItem 

Class

# NSExtensionItem

An immutable collection of values representing different aspects of an item for an extension to act upon.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSExtensionItem
```

## Topics

### Identifying the Item

var attributedTitle: NSAttributedString?

An optional title for the item.

var userInfo: [AnyHashable : Any]?

An optional dictionary of keys and values corresponding to the extension item’s properties.

### Item Contents

var attachments: [NSItemProvider]?

An optional array of media data associated with the extension item.

var attributedContentText: NSAttributedString?

An optional string describing the extension item content.

### Constants

Property Keys

These keys correspond to the extension item properties and are specified in the extension’s `Info.plist`.

UTI Subtypes for Data Detector Types

These constants represent sub-Uniform Type Identifier of `com.apple.structured-text`

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Attachments

class NSItemProvider

An item provider for conveying data or a file between processes during drag-and-drop or copy-and-paste activities, or from a host app to an app extension.

Add Functionality to Finder with Action Extensions

Implement Action Extensions to provide quick access to commonly used features of your app.

