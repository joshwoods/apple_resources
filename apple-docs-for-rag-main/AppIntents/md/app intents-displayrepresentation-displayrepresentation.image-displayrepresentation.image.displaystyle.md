

- App Intents
- DisplayRepresentation
- DisplayRepresentation.Image
-  DisplayRepresentation.Image.DisplayStyle 

Structure

# DisplayRepresentation.Image.DisplayStyle

The style with which to display the image for this `DisplayRepresentation`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct DisplayStyle
```

## Overview

Note that these are only used when an image, not a symbol name, is specified. When symbol names are specified, they are rendered automatically as appropriate for the system.

## Topics

### Operators

static func == (DisplayRepresentation.Image.DisplayStyle, DisplayRepresentation.Image.DisplayStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Type Properties

static var circular: DisplayRepresentation.Image.DisplayStyle

Display this representation in a circle.

static var `default`: DisplayRepresentation.Image.DisplayStyle

Display this representation in the default style.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

