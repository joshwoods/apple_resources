

- PDFKit
- PDFAnnotation
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a bezier path from an ink annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func remove(_ path: UIBezierPath)
```

**macOS**

``` source
func remove(_ path: NSBezierPath)
```

## Parameters 

`path`  

The bezier path to remove, in annotation-space coordinates.

## See Also

### Configuring Ink Annotations

var paths: [UIBezierPath]?

An array of bezier paths, in annotation-space coordinates, that compose the annotation.

func add(UIBezierPath)

Adds a bezier path to the ink annotation.

