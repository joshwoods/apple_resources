

- UIKit
-  UIConfigurationTextAttributesTransformer 

Structure

# UIConfigurationTextAttributesTransformer

Defines a text transformation that can affect the visual appearance of a string.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
struct UIConfigurationTextAttributesTransformer
```

## Overview

Use a transformer to affect how your attributed text appears on the UI. You provide a closure when initializing the transformer. Your closure accepts a container with the current text attributes and returns a container with the new text attributes.

```
let transformer = UIConfigurationTextAttributesTransformer { incoming in
    var outgoing = incoming
    outgoing.foregroundColor = UIColor.black
    outgoing.font = UIFont.boldSystemFont(ofSize: 20)
    return outgoing
}
```

## Topics

### Creating a text attributes transformer

init((AttributeContainer) -> AttributeContainer)

Creates a new text attributes transformer.

### Defining a text transformation

let transform: (AttributeContainer) -> AttributeContainer

A closure that defines the text transformation.

### Calling a text transformer

func callAsFunction(AttributeContainer) -> AttributeContainer

Calls the transform closure of the text attributes transformer.

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

var titlePadding: CGFloat

The distance between the title and subtitle labels.

var titleAlignment: UIButton.Configuration.TitleAlignment

The text alignment the button uses to lay out the title and subtitle.

enum TitleAlignment

Specifies how to align a button’s title and subtitle.

var titleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s title.

var subtitleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s subtitle.

