

- Group Activities
-  SpatialTemplateConfiguration 

Structure

# SpatialTemplateConfiguration

A type that contains the configuration details for a spatial template.

visionOS 2.0+

``` source
struct SpatialTemplateConfiguration
```

## Overview

Create a SpatialTemplateConfiguration structure and fill it with the information you want to apply to your custom SpatialTemplate type. A configuration structure contains the role to give to the person who initiates an activity that uses the template. For example, you might assign a presenter role to a person presenting a slide deck. Spatial templates use roles to place spatial Personas in the shared coordinate space.

## Topics

### Operators

static func == (SpatialTemplateConfiguration, SpatialTemplateConfiguration) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Initializers

init(defaultInitiatorRole: (any SpatialTemplateRole)?)

Creates the configuration structure for a spatial template.

### Instance Properties

let defaultInitiatorRole: (any SpatialTemplateRole)?

The default role to assign to the initiator of the group activity.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring the spatial template

var configuration: SpatialTemplateConfiguration

Information a spatial template uses to configure itself.

**Required** Default implementation provided.

