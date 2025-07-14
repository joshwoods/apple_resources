

- MusicKit
- ArtworkImage
-  symbolEffectsRemoved(\_:) 

Instance Method

# symbolEffectsRemoved(\_:)

Returns a new view with its inherited symbol image effects either removed or left unchanged.

MusicKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func symbolEffectsRemoved(_ isEnabled: Bool = true) -> some View
```

## Parameters 

`isEnabled`  

Whether to remove inherited symbol effects or not.

## Return Value

A copy of the view with its symbol effects either removed or left unchanged.

## Discussion

The following example adds a repeating pulse effect to two symbol images, but then disables the effect on one of them:

```
VStack {
    Image(systemName: "bolt.slash.fill") // does not pulse
        .symbolEffectsRemoved()
    Image(systemName: "folder.fill.badge.person.crop") // pulses
}
.symbolEffect(.pulse)
```

