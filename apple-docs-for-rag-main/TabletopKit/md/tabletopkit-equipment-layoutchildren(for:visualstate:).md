

- TabletopKit
- Equipment
-  layoutChildren(for:visualState:) 

Instance Method

# layoutChildren(for:visualState:)

This function provides the layout of the direct children of this equipment and is called whenever the snapshot changes. Override it to provide a custom layout. The output of this function is considered to be only a function of its inputs. Reaching out to data outside what is provided might result in undefined behavior.

visionOS 2.0+

``` source
func layoutChildren(
    for snapshot: TableSnapshot,
    visualState: TableVisualState
) -> any EquipmentLayout
```

**Required** Default implementation provided.

## Default Implementations

### Equipment Implementations

func layoutChildren(for: TableSnapshot, visualState: TableVisualState) -> any EquipmentLayout

This function provides the layout of the direct children of this equipment and is called whenever the snapshot changes. Override it to provide a custom layout. The output of this function is considered to be only a function of its inputs. Reaching out to data outside what is provided might result in undefined behavior.

## See Also

### Displaying the equipment

func restingOrientation(state: Self.State) -> Rotation3D

The resting orientation of the equipment given the current State.

**Required** Default implementations provided.

