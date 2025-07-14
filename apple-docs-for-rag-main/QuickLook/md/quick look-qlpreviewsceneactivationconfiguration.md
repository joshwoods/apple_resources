

- Quick Look
-  QLPreviewSceneActivationConfiguration 

Class

# QLPreviewSceneActivationConfiguration

A scene configuration to preview items at the specified URLs.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class QLPreviewSceneActivationConfiguration
```

## Overview

This class provides the configuration for a prominent scene presentation of a preview, either from a swipe gesture or a menu action. The user can detach the prominent Quick Look window and display it independently.

To provide a preview from a swipe gesture, use an instance of this class with UIWindowScene.ActivationInteraction. To provide a preview from a menu action, use an instance of this class with UIWindowScene.ActivationAction.

## Topics

### Creating a preview scene activation configuration

init(itemsAt: [URL], options: QLPreviewSceneActivationConfiguration.Options?)

Creates a preview scene configuration.

### Configuring a preview scene activation

class Options

A class that represents the configuration for a preview scene activation.

## Relationships

### Inherits From

- UIWindowScene.ActivationConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Previews

class QLPreviewController

A specialized view controller for previewing an item.

protocol QLPreviewItem : NSObjectProtocol

A protocol that defines a set of properties you implement to make a preview of your application’s content.

Previews or thumbnail images for macOS 10.14 or earlier

Create thumbnail images or previews of common files and custom file types in earlier versions of macOS.

