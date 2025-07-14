

- PDFKit
- PDFAnnotation
-  paths 

Instance Property

# paths

An array of bezier paths, in annotation-space coordinates, that compose the annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

**macOS**

``` source
var paths: [NSBezierPath]? { get }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var paths: [UIBezierPath]? { get }
```

## See Also

### Configuring Ink Annotations

func add(UIBezierPath)

Adds a bezier path to the ink annotation.

func remove(UIBezierPath)

Removes a bezier path from an ink annotation.

