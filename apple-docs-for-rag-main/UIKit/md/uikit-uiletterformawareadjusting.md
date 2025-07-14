

- UIKit
-  UILetterformAwareAdjusting 

Protocol

# UILetterformAwareAdjusting

The typographic bounds-sizing behavior to handle text with fonts that contain oversize characters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UILetterformAwareAdjusting : NSObjectProtocol
```

## Overview

In UILabel, UITextField, or a nonscrollable UITextView, sizeThatFits(_:) and intrinsicContentSize increase the height calculated for tall scripts when you present text that contains oversize characters in a font that you create with preferredFont(forTextStyle:). Even with the increase, some extreme ascenders and descenders may extend beyond the view’s bounds and appear to be clipped. For nontext-style fonts, sizeThatFits(_:) and intrinsicContentSize don’t increase the calculated height for oversize characters. This is the default, standard behavior. Set sizingRule to UILetterformAwareSizingRule.typographic to use this behavior explicitly.

To adjust the boundary calculations in sizeThatFits(_:) and intrinsicContentSize to account for oversize characters, set sizingRule to UILetterformAwareSizingRule.oversize. Note that the larger bounds to accommodate oversize characters may negatively impact typographic alignment, such as vertical edge alignment, vertical edge-to-edge spacing, or vertical centering.

## Topics

### Specifying text-sizing behavior

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

enum UILetterformAwareSizingRule

Constants that specify typographic bounds-sizing behavior to handle text in fonts with oversize characters.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UILabel
- UISearchTextField
- UITextField
- UITextView

