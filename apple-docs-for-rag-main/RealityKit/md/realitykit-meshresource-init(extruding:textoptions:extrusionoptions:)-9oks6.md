

- RealityKit
- MeshResource
-  init(extruding:textOptions:extrusionOptions:) 

Initializer

# init(extruding:textOptions:extrusionOptions:)

Asynchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
convenience init(
    extruding string: AttributedString,
    textOptions: MeshResource.GenerateTextOptions = GenerateTextOptions(),
    extrusionOptions: MeshResource.ShapeExtrusionOptions = ShapeExtrusionOptions()
) async throws
```

## Parameters 

`string`  

A string that contains text for the 3D mesh geometry.

`textOptions`  

A configuration for rendering the text in 2D, before extrusion.

`extrusionOptions`  

A configuration for extruding the text in 3D.

## Discussion

You can use the method to make a 3D mesh of a string, control the text’s layout, chamfers, materials, and how to extrude the shape into 3D.

The generated text is scaled at a ratio of 72 points per meter.

## See Also

### Creating a text mesh resource

static func generateText(String, extrusionDepth: Float, font: MeshResource.Font, containerFrame: CGRect, alignment: CTTextAlignment, lineBreakMode: CTLineBreakMode) -> MeshResource

Generates a 3D mesh for rendering static text.

static func generateText(String, extrusionDepth: Float, font: MeshResource.Font, containerFrame: CGRect, alignment: CTTextAlignment, lineBreakMode: CTLineBreakMode) -> MeshResource

Generates a 3D mesh for rendering static text.

convenience init(extruding: AttributedString, textOptions: MeshResource.GenerateTextOptions, extrusionOptions: MeshResource.ShapeExtrusionOptions) throws

Synchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

