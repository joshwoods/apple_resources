

- App Intents
- ShortcutsLink
-  allowedDynamicRange(\_:) 

Instance Method

# allowedDynamicRange(\_:)

Returns a new view configured with the specified allowed dynamic range.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func allowedDynamicRange(_ range: Image.DynamicRange?) -> some View
```

## Parameters 

`range`  

The requested dynamic range, or nil to restore the default allowed range.

## Return Value

A new view.

## Discussion

The following example enables HDR rendering within a view hierarchy:

```
MyView().allowedDynamicRange(.high)
```

