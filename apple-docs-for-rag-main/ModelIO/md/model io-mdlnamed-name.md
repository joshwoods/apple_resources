

- Model I/O
- MDLNamed
-  name 

Instance Property

# name

A descriptive name for the object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var name: String { get set }
```

**Required**

## Discussion

Many types of Model I/O objects support this property. For objects loaded from a file using the MDLAsset class, this property may reflect the name or label assigned by an artist using 3D authoring tools.

