

- Group Activities
-  SpatialTemplateElementAxis 

Structure

# SpatialTemplateElementAxis

An axis to use when aligning elements in a spatial template.

visionOS 2.0+

``` source
struct SpatialTemplateElementAxis
```

## Overview

When configuring the elements of a spatial template, you can specify directions that orient a participant with the x- or z-axis of the shared coordinate space. These alignments rotate the participant around the y-axis to face the specified axis.

## Topics

### Operators

static func == (SpatialTemplateElementAxis, SpatialTemplateElementAxis) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let x: SpatialTemplateElementAxis

The x-axis of alignment.

static let z: SpatialTemplateElementAxis

The z-axis of alignment.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Looking along an axis

static func alignedWith(appAxis: SpatialTemplateElementAxis) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to look along the specified axis in the direction of the app’s content.

