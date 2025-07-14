

- TabletopKit
- TabletopInteraction
-  TabletopInteraction.Destination 

Structure

# TabletopInteraction.Destination

An object that represents the destination position and orientation of equipment in an interaction.

visionOS 2.0+

``` source
struct Destination
```

## Overview

The position and orientation can be relative to either a piece of equipment or the table.

## Topics

### Getting the destination equipment

let equipmentID: EquipmentIdentifier

The interaction’s destination equipment.

### Getting the interaction pose

let pose: TableVisualState.Pose2D

The 2D position and orientation of the interaction.

## Relationships

### Conforms To

- Sendable

## See Also

### Managing the interaction destination

func setAllowedDestinations(TabletopInteraction.AllowedDestinations)

Sets which equipment the interaction can target.

Deprecated

enum AllowedDestinations

The possible destinations of equipment in an interaction.

