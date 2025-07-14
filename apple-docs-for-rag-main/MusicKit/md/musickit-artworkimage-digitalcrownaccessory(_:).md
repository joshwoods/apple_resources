

- MusicKit
- ArtworkImage
-  digitalCrownAccessory(\_:) 

Instance Method

# digitalCrownAccessory(\_:)

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

MusicKitSwiftUIwatchOS 9.0+

``` source
nonisolated
func digitalCrownAccessory(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

The visibility of the digital crown accessory.

## Discussion

Use this method to customize the visibility of a Digital Crown accessory `View` created with the `View/digitalCrownAccessory(_ content:)` modifier. You may want to keep an accessory visible even when the Digital Crown Indicator is not visible to indicate what scrolling the crown will do.

