

- TabletopKit
-  Tabletop 

Protocol

# Tabletop

A protocol for the table surface in your game.

visionOS 2.0+

``` source
protocol Tabletop : Identifiable where Self.ID == EquipmentIdentifier
```

## Overview

To create a TableSetup object that configures your game table, pass an object that conforms to either the `Tabletop` or ``` EntityTabletop`` protocol to the  ```TableSetup`initializer. Implement your`Tabletop`structure to set the protocol properties, such as the`shape`and`id\` properties.

```
struct Table: Tabletop {
    var shape = .rectangular(width: 100, height: 60, thickness: 5, in: .centimeters)
    var id = .table
}
```

To create a round table, use one of the TabletopShape round initializers.

To render the table surface using RealityKit, conform to the EntityTabletop protocol instead.

## Topics

### Creating a round or rectangular table

var shape: TabletopShape

**Required** Default implementation provided.

### Displaying the equipment

func layoutChildren(for: TableSnapshot, visualState: TableVisualState) -> any EquipmentLayout

This function provides the layout of the direct children of this equipment and is called whenever the snapshot changes. Override it to provide a custom layout. The output of this function is considered to be only a function of its inputs. Reaching out to data outside what is provided might result in undefined behavior.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Identifiable

### Inherited By

- EntityTabletop

## See Also

### Essentials

Creating tabletop games

Develop a spatial board game where multiple players interact with pieces on a table.

class TabletopGame

An object that manages the setup and gameplay of a tabletop game.

struct TableSetup

An object that represents the arrangement of seats, equipment, and counters around the game table.

protocol EntityTabletop

A protocol for the table surface in your game when you render it using RealityKit.

struct TabletopShape

An object that represents the physical properties of the table.

