

- Group Activities
-  SpatialTemplatePreference 

Structure

# SpatialTemplatePreference

A structure that specifies the preferred arrangement of participant spatial Personas in a shared simulation space.

visionOS 1.0+

``` source
struct SpatialTemplatePreference
```

## Overview

Use the static members of this structure to specify your preferred arrangement of participants around your app’s content. The system applies your preference only when displaying spatial Personas in the scene.

## Topics

### Getting the spatial position preferences

static let none: SpatialTemplatePreference

An arrangement where the system places spatial Personas based on your app’s content.

static let sideBySide: SpatialTemplatePreference

An arrangement where the participants sit in a line with the content in front of them.

static let conversational: SpatialTemplatePreference

An arrangement where the participants can see one another and the app’s content.

static func custom(any SpatialTemplate) -> SpatialTemplatePreference

Creates a template preference with the given custom spatial template.

### Specifying the distance between content and participants

func contentExtent(CGFloat) -> SpatialTemplatePreference

Sets the distance between the app’s content and any participants.

### Getting the template description

var description: String

A textual representation of this instance.

### Type Properties

static let surround: SpatialTemplatePreference

An arrangement where the participants sit around the content.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Specifying spatial position preferences

var spatialTemplatePreference: SpatialTemplatePreference

The preferred arrangement of spatial Personas in your app’s immersive space.

