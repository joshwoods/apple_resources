

- BrowserEngineKit
-  BEContextMenuConfiguration 

Class

# BEContextMenuConfiguration

A specialized `UIContextMenuConfiguration` object to defer a context menu presentation when the when the context menu gestures are first recognized and a possible menu presentation is not immediately known.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
class BEContextMenuConfiguration
```

## Overview

An object that defers presentation of the contextual menu.

## Overview

Return an instance of this object if you don’t know whether presentation of a contextual menu is possible, or don’t already have the menu items when the system calls your interaction delegate’s contextMenuInteraction(_:configurationForMenuAtLocation:) method. As soon as you have the real configuration, call fulfill(using:), and pass the real configuration as the parameter, or `nil` to indicate no menu presentation is possible.

Note

In most situations, use UIDeferredMenuElement if you don’t have the content of a contextual menu element when the system asks your delegate and you need to calculate it asynchronously. When calculating the contextual menu configuration involves a short deferral, for example, making an XPC call to a browser extension, use `BEContextMenuConfiguration` instead.

## Topics

### Creating a context menu configuration

init()

Creates a new configuration for the context menu interaction.

### Fulfilling the configuration

func fulfill(using: UIContextMenuConfiguration?) -> Bool

Fulfills the configuration with a concrete configuration. Once fulfilled, the context menu presentation will begin. You should call this method as soon as you have determined that a menu presentation is possible for the configuration, as to minimize the delay between the context menu gesture’s recognition and the menu’s presentation. If no menu presentation is possible, fulfill with a `nil` configuration.

## Relationships

### Inherits From

- UIContextMenuConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

