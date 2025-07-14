

- File Provider
-  NSFileProviderItemDecorating 

Protocol

# NSFileProviderItemDecorating

Support for decorating items.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderItemDecorating : NSFileProviderItemProtocol
```

## Overview

To adopt this protocol, implement the decorations method for your extension’s NSFileProviderItem and return valid identifiers for the desired decorations.

You define decorations in the File Provider extension’s `Info.plist` file by adding the `NSFileProviderDecorations` key to the `NSExtension` dictionary.

```
 NSFileProviderDecorations

      Identifier
      $(PRODUCT_BUNDLE_IDENTIFIER).hasComments
      BadgeImageType
      com.someone.item.decoration.unreadCommentIcon
      Category
      Badge
      LocalizedTitle

         NSStringFormat
         %@ unread comments
         NSStringFormatValues

            item.userInfo.unreadCommentCount

```

Use the following keys to define the decorations:

`Identifier`  
The decoration’s identifier.

`BadgeImageType`  
A UTI for the item’s badge. To define the badge, create a new UTI that conforms to `com.apple.icon-decoration.badge` and set its icon.

`Label`  
A localizable title for the item. For example, the system displays a title in detail views and VoiceOver.

`Category`  
A string that defines the location of the badge image.

The `Category` value must be one of the following:

`Badge`  
The system displays the badge image on top of the item’s icon. It only displays the first `Badge` image.

`Sharing`  
The system displays the badge image below the icon. It only displays the first `Sharing` image.

`FolderBadge`  
Only available on folder items. The system embosses the image over the folder icon. It only displays the first `FolderBadge` image.

## Topics

### Providing Decorations

var decorations: [NSFileProviderItemDecorationIdentifier]?

Asks the item for an array of decorations.

**Required**

## Relationships

### Inherits From

- NSFileProviderItemProtocol
- NSObjectProtocol

## See Also

### Items and metadata

struct NSFileProviderItemFields

Fields that specify which of the item’s properties have changed.

class NSFileProviderItemVersion

The version of the item’s content and its metadata.

class NSFileProviderRequest

An object that provides information about the application requesting data from the File Provider extension.

struct NSFileProviderItemDecorationIdentifier

A decoration identifier defined in the File Provider extension’s information property list.

