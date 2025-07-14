

- Core Location
- CLMonitor
-  CLMonitor.CircularGeographicCondition 

Structure

# CLMonitor.CircularGeographicCondition

A condition that describes a circular geographic area that a center point and radius define.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct CircularGeographicCondition
```

## Overview

Use `CLMonitor.CircularGeographicCondition` to monitor events that occur in a circular geographic condition that you describe.

## Topics

### Creating a circular geographic condition

init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates a circular geographic condition with a center point and radius you specify.

### Condition characteristics

let center: CLLocationCoordinate2D

The center point of the condition’s area.

let radius: CLLocationDistance

The radius of the condition’s area, in meters.

## Relationships

### Conforms To

- CLCondition
- Decodable
- Encodable
- Sendable

## See Also

### Monitor conditions

struct BeaconIdentityCondition

A condition that describes the characteristics of a beacon.

