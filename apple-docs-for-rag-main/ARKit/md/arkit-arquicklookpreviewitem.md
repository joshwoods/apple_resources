

- ARKit
-  ARQuickLookPreviewItem 

Class

# ARQuickLookPreviewItem

An object for customizing the AR Quick Look experience.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARQuickLookPreviewItem
```

## Mentioned in 

Previewing a Model with AR Quick Look

## Overview

Use this class when you want to control the background, designate which content the share sheet shares, or disable scaling in case it’s not appropriate to allow the user to scale a particular model.

## Topics

### Creating a Preview Item

init(fileAt: URL)

Initializes a new AR Quick Look preview item.

### Scaling Content

var allowsContentScaling: Bool

A Boolean value that determines whether the user can scale your virtual content using pinch gestures.

### Interacting with Content

var canonicalWebPageURL: URL?

The web URL to share when the user invokes the share sheet.

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
- QLPreviewItem

## See Also

### AR Quick Look

Previewing a Model with AR Quick Look

Display a model or scene that the user can move, scale, and share with others.

Adding Visual Effects in AR Quick Look and RealityKit

Balance the appearance and performance of your AR experiences with modeling strategies.

Adding an Apple Pay Button or a Custom Action in AR Quick Look

Provide a banner that users can tap to make a purchase or perform a custom action in an AR experience.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

