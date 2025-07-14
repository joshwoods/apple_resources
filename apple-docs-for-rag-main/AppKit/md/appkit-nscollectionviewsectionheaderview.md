

- AppKit
-  NSCollectionViewSectionHeaderView 

Protocol

# NSCollectionViewSectionHeaderView

A protocol that defines a button to control the collapse of a collection view’s section.

macOS

``` source
protocol NSCollectionViewSectionHeaderView : NSCollectionViewElement
```

## Overview

A collection view can support a section that can collapse into a single horizontally scrollable row, similar to the groupings in the icon view in Finder. To ensure that the collection view can communicate with the button that controls the collapsing of a section, the section header view object should conform to this protocol and connect the button’s outlet to sectionCollapseButton.

## Topics

### Providing a Collapse Button

var sectionCollapseButton: NSButton?

A control that lets users collapse and open a collection view section.

## Relationships

### Inherits From

- NSCollectionViewElement
- NSObjectProtocol
- NSUserInterfaceItemIdentification

## See Also

### View

class NSCollectionView

An ordered collection of data items displayed in a customizable layout.

