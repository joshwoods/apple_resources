

- UIKit
- UINavigationItem
-  UINavigationItem.ItemStyle 

Enumeration

# UINavigationItem.ItemStyle

Constants that determine how the content of the navigation item lays out in the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum ItemStyle
```

## Overview

Navigation styles allow you to customize the behavior and content density of your navigation bar according to your app type.

- Navigator apps like Settings support a traditional navigation model for hierarchical data.

- Browser apps like Safari or Files support browsing through and navigating back and forth between multiple documents or folder structures.

- Editor apps support focused viewing or editing of individual documents.

Related Sessions from WWDC22

Session 10069: Meet desktop-class iPad

Session 10070: Build a desktop-class iPad app

## Topics

### Constants

case navigator

A style for a traditional navigation-based interface.

case browser

A style for a browser app interface.

case editor

A style for an editor app interface.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the navigation style

var style: UINavigationItem.ItemStyle

A style that determines how the content of the navigation item lays out in the navigation bar.

