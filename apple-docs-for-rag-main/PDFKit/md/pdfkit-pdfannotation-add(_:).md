

- PDFKit
- PDFAnnotation
-  add(\_:) 

Instance Method

# add(\_:)

Adds a bezier path to the ink annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func add(_ path: UIBezierPath)
```

**macOS**

``` source
func add(_ path: NSBezierPath)
```

## Parameters 

`path`  

The bezier path to add, in annotation-space coordinates.

## See Also

### Configuring Ink Annotations

var paths: [UIBezierPath]?

An array of bezier paths, in annotation-space coordinates, that compose the annotation.

func remove(UIBezierPath)

Removes a bezier path from an ink annotation.

