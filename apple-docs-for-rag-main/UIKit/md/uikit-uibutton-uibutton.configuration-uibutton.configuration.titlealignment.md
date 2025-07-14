

- UIKit
- UIButton
- UIButton.Configuration
-  UIButton.Configuration.TitleAlignment 

Enumeration

# UIButton.Configuration.TitleAlignment

Specifies how to align a button’s title and subtitle.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
enum TitleAlignment
```

## Overview

If your button displays both title and subtitle, use this enumeration to configure how the text aligns.

## Topics

### Title alignments

case automatic

Aligns the title and subtitle based on other elements in the button configuration, like an image or activity indicator.

case center

Aligns the title and subtitle on their horizontal centers.

case leading

Aligns the title and subtitle on their leading edges.

case trailing

Aligns the title and subtitle on their trailing edges.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring titles

var title: String?

The text of the title label the button displays.

var subtitle: String?

The text the subtitle label of the button displays.

var attributedTitle: AttributedString?

The text and style attributes for the button’s title label.

var attributedSubtitle: AttributedString?

The text and style attributes for the button’s subtitle label.

var titleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed title when the button state changes.

var subtitleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed subtitle when the button state changes.

struct UIConfigurationTextAttributesTransformer

Defines a text transformation that can affect the visual appearance of a string.

var titlePadding: CGFloat

The distance between the title and subtitle labels.

var titleAlignment: UIButton.Configuration.TitleAlignment

The text alignment the button uses to lay out the title and subtitle.

var titleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s title.

var subtitleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s subtitle.

