

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  accessibilityValue(\_:) 

Instance Method

# accessibilityValue(\_:)

Adds a textual description of the value that the view contains.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityValue(_ valueKey: LocalizedStringKey) -> ModifiedContent
```

## Discussion

Use this method to describe the value represented by a view, but only if that’s different than the view’s label. For example, for a slider that you label as “Volume” using accessibilityLabel(), you can provide the current volume setting, like “60%”, using accessibilityValue().

