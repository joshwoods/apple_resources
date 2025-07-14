

- RealityKit
- MeshResource
-  generateText(\_:extrusionDepth:font:containerFrame:alignment:lineBreakMode:) 

Type Method

# generateText(\_:extrusionDepth:font:containerFrame:alignment:lineBreakMode:)

Generates a 3D mesh for rendering static text.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateText(
    _ string: String,
    extrusionDepth: Float = 0.25,
    font: MeshResource.Font = .systemFont(ofSize: MeshResource.Font.systemFontSize),
    containerFrame: CGRect = CGRect.zero,
    alignment: CTTextAlignment = .left,
    lineBreakMode: CTLineBreakMode = .byTruncatingTail
) -> MeshResource
```

## Parameters 

`string`  

The text to render.

`extrusionDepth`  

The extent, in meters, of the extruded text in the z-axis direction.

`font`  

The font to use. The font size is in meters.

`containerFrame`  

The size, in meters, of the text frame in the local coordinate system where the text is laid out. The text frame has the same origin as the local coordinate system.

Use a frame size of `(0,0)` to tell the method to create a frame large enough to contain the generated text.

`alignment`  

How the text should be aligned in the text frame.

`lineBreakMode`  

How the text should wrap when reaching a frame boundary.

## Return Value

The text mesh.

## See Also

### Creating a text mesh resource

static func generateText(String, extrusionDepth: Float, font: MeshResource.Font, containerFrame: CGRect, alignment: CTTextAlignment, lineBreakMode: CTLineBreakMode) -> MeshResource

Generates a 3D mesh for rendering static text.

convenience init(extruding: AttributedString, textOptions: MeshResource.GenerateTextOptions, extrusionOptions: MeshResource.ShapeExtrusionOptions) async throws

Asynchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

convenience init(extruding: AttributedString, textOptions: MeshResource.GenerateTextOptions, extrusionOptions: MeshResource.ShapeExtrusionOptions) throws

Synchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

