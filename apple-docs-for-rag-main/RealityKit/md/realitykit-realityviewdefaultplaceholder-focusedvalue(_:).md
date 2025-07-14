

- RealityKit
- RealityViewDefaultPlaceholder
-  focusedValue(\_:) 

Instance Method

# focusedValue(\_:)

Sets the focused value for the given object type.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func focusedValue(_ object: T?) -> some View where T : AnyObject, T : Observable
```

## Discussion

Important

This initializer only accepts objects conforming to the `Observable` protocol. For reading environment objects that conform to `ObservableObject`, use `focusedObject(_:)`, instead.

To read this value, use the `FocusedValue` property wrapper.

