

- TV Services
-  Legacy Extension 

API Collection

# Legacy Extension

Help users discover your app by providing top shelf content and a description of your tvOS app.

## Overview

In iOS 12 and earlier, you provide Top Shelf information by adding a TVServices app extension to your app. Your extension returns an array describing available content for your app, and the system uses this information to update the Top Shelf. You describe your media to the operating system using TVContentItem objects. Each TVContentItem object represents either a piece of content or acts as a container for other TVContentItem objects. A content object typically includes an image and a title for tvOS to display, along with other metadata related to the content item.

Important

The memory limits for Top Shelf extensions are significantly lower than the memory limits imposed on tvOS apps. Performing memory-intensive operations in a Top Shelf extension, such as image editing or compositing, could push your extension beyond the high-water mark and force it to be terminated. If you must perform cpu-intensive or memory-intensive operations to generate Top Shelf content, perform those operations on a server and provide URLs to the generated resources. For more information on creating extensions, see App Extension Programming Guide.

In order for tvOS to track content items, you create a unique string for each content item. You can choose your own algorithm to create these identifiers. However, any string you create should identify its content item forever; never recycle identifiers for new content. You package an identifier in a TVContentIdentifier object, which includes the string and the parent container of the item.

To summarize, to provide descriptions of content to Apple TV, you must:

- Organize your media and app content, either as a single list or in a hierarchical model

- Design an algorithm or standard that supplies each content item with a unique content identifier string

- Create a TVContentItem object for each container or content item

- Add an app extension whose main class implements the TVTopShelfProvider protocol

## Topics

### Extension

protocol TVTopShelfProvider

The interface for providing items to display in the main menu’s Top Shelf user interface on an Apple TV.

Deprecated

### Content

class TVContentItem

An object that describes either a piece of content or a container for other content items.

Deprecated

class TVContentIdentifier

An object that uniquely identifies media content in either a single piece or a collection.

Deprecated

func TVTopShelfImageSize(shape: TVContentItemImageShape, style: TVTopShelfContentStyle) -> CGSize

Returns the ideal size for an image, according to its particular shape and style.

Deprecated

## See Also

### Top shelf app extensions

Building a Full Screen Top Shelf Extension

Highlight content from your Apple TV application by building a full screen Top Shelf extension.

class TVTopShelfContentProvider

The main interface for your Top Shelf app extension, which you use to provide content for the top shelf area of the tvOS Home Screen.

