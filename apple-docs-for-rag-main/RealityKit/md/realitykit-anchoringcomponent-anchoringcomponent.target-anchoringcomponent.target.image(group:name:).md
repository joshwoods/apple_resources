

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.image(group:name:) 

Case

# AnchoringComponent.Target.image(group:name:)

An anchor point attached to the image specified by a group and a name in AR Resources.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
case image(
    group: String,
    name: String
)
```

## See Also

### Image and object anchor targets

case referenceImage(from: AnchoringComponent.ImageAnchoringSource)

An anchor point attached to the image specified by an image anchoring source.

case object(group: String, name: String)

An anchor point attached to the object specified by a group and a name in AR Resources.

case referenceObject(from: AnchoringComponent.ObjectAnchoringSource)

An anchor point attached to the object specified by an object anchoring source.

