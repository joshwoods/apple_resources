

- RealityKit
- Model3D
-  accessibilityTextContentType(\_:) 

Instance Method

# accessibilityTextContentType(\_:)

Sets an accessibility text content type.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func accessibilityTextContentType(_ value: AccessibilityTextContentType) -> ModifiedContent
```

## Parameters 

`value`  

The accessibility content type from the available `AccessibilityTextContentType` options.

## Discussion

Use this modifier to set the content type of this accessibility element. Assistive technologies can use this property to choose an appropriate way to output the text. For example, when encountering a source coding context, VoiceOver could choose to speak all punctuation.

The default content type `AccessibilityTextContentType/plain`.

