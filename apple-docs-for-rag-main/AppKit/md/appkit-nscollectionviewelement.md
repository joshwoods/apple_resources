

- AppKit
-  NSCollectionViewElement 

Protocol

# NSCollectionViewElement

A set of methods that you use to manage the content in a collection view.

macOS

``` source
protocol NSCollectionViewElement : NSUserInterfaceItemIdentification, NSObjectProtocol
```

## Overview

Adopt this protocol in the classes that you use to display content for items, supplementary views, and decoration views in a collection view. The methods of this protocol are optional and provide support for applying layout attributes and for cleaning up elements when they move offscreen and are recycled.

Collection view items—that is, instances of the NSCollectionViewItem class—already adopt this protocol. For supplementary and decoration views, adopt this protocol in the custom view classes you use to represent that content.

## Topics

### Reusing Elements

func prepareForReuse()

Performs any necessary cleanup to prepare the element for use again.

### Managing Layout Changes

func preferredLayoutAttributesFitting(NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutAttributes

Asks your element if it wants to modify any layout attributes before they are applied.

func apply(NSCollectionViewLayoutAttributes)

Applies the specified layout attributes to the element.

func willTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view is about to change.

func didTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view changed.

## Relationships

### Inherits From

- NSObjectProtocol
- NSUserInterfaceItemIdentification

### Inherited By

- NSCollectionViewSectionHeaderView

### Conforming Types

- NSCollectionViewItem

## See Also

### Items

class NSCollectionViewItem

The visual representation for a single data element in a collection view.

