

- TabletopKit
- Equipment
-  restingOrientation(state:) 

Instance Method

# restingOrientation(state:)

The resting orientation of the equipment given the current State.

visionOS 2.0+

``` source
func restingOrientation(state: Self.State) -> Rotation3D
```

**Required** Default implementations provided.

## Default Implementations

### Equipment Implementations

func restingOrientation(state: Self.State) -> Rotation3D

The resting orientation of the equipment given the current State.

func restingOrientation(state: Self.State) -> Rotation3D

The resting orientation of the equipment given the current State.

## See Also

### Displaying the equipment

func layoutChildren(for: TableSnapshot, visualState: TableVisualState) -> any EquipmentLayout

This function provides the layout of the direct children of this equipment and is called whenever the snapshot changes. Override it to provide a custom layout. The output of this function is considered to be only a function of its inputs. Reaching out to data outside what is provided might result in undefined behavior.

**Required** Default implementation provided.

