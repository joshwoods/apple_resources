

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.object(group:name:) 

Case

# AnchoringComponent.Target.object(group:name:)

An anchor point attached to the object specified by a group and a name in AR Resources.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
case object(
    group: String,
    name: String
)
```

## See Also

### Image and object anchor targets

case image(group: String, name: String)

An anchor point attached to the image specified by a group and a name in AR Resources.

case referenceImage(from: AnchoringComponent.ImageAnchoringSource)

An anchor point attached to the image specified by an image anchoring source.

case referenceObject(from: AnchoringComponent.ObjectAnchoringSource)

An anchor point attached to the object specified by an object anchoring source.

