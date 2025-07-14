

- TabletopKit
- TabletopInteraction
-  TabletopInteraction.AllowedDestinations 

Enumeration

# TabletopInteraction.AllowedDestinations

The possible destinations of equipment in an interaction.

visionOS 2.0+

``` source
enum AllowedDestinations
```

## Topics

### Destinations

case any

Any equipment is allowed to be the proposed destination

case restricted([EquipmentIdentifier])

Restricts the proposed destination to the given identifiers

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Managing the interaction destination

func setAllowedDestinations(TabletopInteraction.AllowedDestinations)

Sets which equipment the interaction can target.

Deprecated

struct Destination

An object that represents the destination position and orientation of equipment in an interaction.

