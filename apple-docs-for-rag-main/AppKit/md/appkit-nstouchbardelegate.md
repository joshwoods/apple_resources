

- AppKit
-  NSTouchBarDelegate 

Protocol

# NSTouchBarDelegate

A protocol that allows you to provide the items for a bar dynamically.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
protocol NSTouchBarDelegate : NSObjectProtocol
```

## Overview

Use a bar delegate, according to the needs of your app, to dynamically create items (NSTouchBarItem instances). For more information, see Item objects.

## Topics

### Providing bar items

func touchBar(NSTouchBar, makeItemForIdentifier: NSTouchBarItem.Identifier) -> NSTouchBarItem?

Asks the delegate object for the bar item for the specified bar and item identifier.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextView

## See Also

### Essentials

Integrating a Toolbar and Touch Bar into Your App

Provide users quick access to your app’s features from a toolbar and corresponding Touch Bar.

Creating and Customizing the Touch Bar

Adopt Touch Bar support by displaying interactive content and controls for your macOS apps.

class NSTouchBar

An object that provides dynamic contextual controls in the Touch Bar of supported models of MacBook Pro.

protocol NSTouchBarProvider

A protocol that an object adopts to create a bar object in your app.

