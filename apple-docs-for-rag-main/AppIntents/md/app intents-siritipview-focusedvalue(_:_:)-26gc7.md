

- App Intents
- SiriTipView
-  focusedValue(\_:\_:) 

Instance Method

# focusedValue(\_:\_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

AppIntentsSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func focusedValue(
    _ keyPath: WritableKeyPath,
    _ value: Value
) -> some View
```

## Parameters 

`keyPath`  

The key path to associate `value` with when adding it to the existing table of exported focus values.

`value`  

The focus value to export.

## Return Value

A modified representation of this view.

