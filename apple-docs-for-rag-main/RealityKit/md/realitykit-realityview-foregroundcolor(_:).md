

- RealityKit
- RealityView
-  foregroundColor(\_:) 

Instance Method

# foregroundColor(\_:)

Sets the color of the foreground elements displayed by this view.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac CatalystmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func foregroundColor(_ color: Color?) -> some View
```

## Parameters 

`color`  

The foreground color to use when displaying this view. Pass `nil` to remove any custom foreground color and to allow the system or the container to provide its own foreground color. If a container-specific override doesn’t exist, the system uses the primary color.

## Return Value

A view that uses the foreground color you supply.

