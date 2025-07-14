

- TabletopKit
-  EntityTabletop 

Protocol

# EntityTabletop

A protocol for the table surface in your game when you render it using RealityKit.

TabletopKitRealityKitvisionOS 2.0+

``` source
protocol EntityTabletop : Tabletop
```

## Overview

To create a TableSetup object that configures your game table, pass an object that conforms to either the Tabletop or `EntityTabletop` protocol to the `TableSetup` initializer. If you render your table surface using RealityKit, conform to the `EntityTabletop` protocol. Implement your `EntityTabletop` structure to set the protocol properties, such as the `shape`, `entity`, and `id` properties.

```
struct Table: EntityTabletop {
    var shape: TabletopShape
    var entity: Entity
    var id: EquipmentIdentifier

    init() {
        self.entity = try! Entity.load(named: "table/table", in: contentBundle)
        self.shape = .round(entity: entity)
        self.id = .table
    }
}
```

## Topics

### Creating a round or rectangular table

var shape: TabletopShape

### Displaying the tabletop

var entity: Entity

The entity associated with the equipment.

**Required**

## Relationships

### Inherits From

- Identifiable
- Tabletop

## See Also

### Essentials

Creating tabletop games

Develop a spatial board game where multiple players interact with pieces on a table.

class TabletopGame

An object that manages the setup and gameplay of a tabletop game.

struct TableSetup

An object that represents the arrangement of seats, equipment, and counters around the game table.

protocol Tabletop

A protocol for the table surface in your game.

struct TabletopShape

An object that represents the physical properties of the table.

