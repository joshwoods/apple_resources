

- Contacts UI
- ContactAccessButton
-  ContactAccessButton.Style 

Structure

# ContactAccessButton.Style

A type that customizes the style of a contact access button.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
struct Style
```

## Overview

This type accounts for a contact access button’s visual traits like color and sizing of the contact image. Set the style of a contact access button with the contactAccessButtonStyle(_:) view modifier.

## Topics

### Creating a style instance

init(imageTrailingEdgePadding: CGFloat?, imageWidth: CGFloat?, imageColor: Color?)

Creates a contact access button with the provided styling values.

### Working with common styles

static let automatic: ContactAccessButton.Style

A style that provides the default system styling of a contact access button.

