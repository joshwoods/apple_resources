

- RealityKit
- USD Assets
- USDZ schemas for AR
-  Preliminary_Text 

# Preliminary_Text

A prim that renders 3D text in a scene.

## Overview

Because `Preliminary_Text` prim is an `Xformable` prim, you define its position either by specifying an offset in world coordinates, or by specifying that the prim should inherit its parent transform.

Alternatively, you can request that the runtime anchor a text prim in the real world by inheriting `Preliminary_AnchoringAPI`. Many AR experiences include anchored text to add information or context about real-world objects or virtual content.

### Declaration

```
class Preliminary_Text "Preliminary_Text" (
    inherits = 
)
```

### Create single-line or flowing text

The following example demonstrates single-line text.

```
def Preliminary_Text "heading"
{
    string content = "Units Sold"
    string[] font = [ "Helvetica", "Arial" ]
    token wrapMode = "singleLine"
    token horizontalAlignment = "left"
    token verticalAlignment = "baseline"
}
```

The following example shows text flowing in a rectangular region, with line breaks as needed.

```
def Preliminary_Text "sign"
{
    string content = "Now is the time for all good people to come to the aid of their country."
    string[] font = [ "ZapfChancery", "Bradley Hand", "cursive" ]
    token wrapMode = "flowing"
    float width = 120
    float height = 100
    token horizontalAlignment = "center"
    token verticalAlignment = "top"
}
```

## Topics

### Properties

content

The characters that the text displays.

font

An array of font names.

pointSize

The size of the text’s font.

width

The width of the text’s bounding box.

height

The height of the text’s bounding box.

depth

A value that defines the depth, in scene units, of the text’s extrusion.

wrapMode

An option that determines the flow of the text.

horizontalAlignment

An option that controls the text’s horizontal placement within its bounding box.

verticalAlignment

An option that controls the text’s vertical placement within its bounding rectangle.

