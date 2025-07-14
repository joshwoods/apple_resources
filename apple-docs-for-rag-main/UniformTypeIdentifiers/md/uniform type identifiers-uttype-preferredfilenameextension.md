

- Uniform Type Identifiers
- UTType
-  preferredFilenameExtension 

Instance Property

# preferredFilenameExtension

The preferred filename extension for the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var preferredFilenameExtension: String? { get }
```

## Discussion

If available, the preferred (first available) tag of class filenameExtension.

Many types require the generation of a filename; for example, when saving a file to disk. If not `nil`, the value of this property is the best available filename extension for this type.

The value of this property is equivalent to, but more efficient than:

```
type.tags[.filenameExtension]?.first
```

## See Also

### Obtaining tags

var preferredMIMEType: String?

The preferred MIME type for the type.

var tags: [UTTagClass : [String]]

The tag specification dictionary of the type.

