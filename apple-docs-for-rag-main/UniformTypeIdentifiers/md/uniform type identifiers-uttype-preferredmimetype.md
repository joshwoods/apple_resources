

- Uniform Type Identifiers
- UTType
-  preferredMIMEType 

Instance Property

# preferredMIMEType

The preferred MIME type for the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var preferredMIMEType: String? { get }
```

## Discussion

If available, the preferred (first available) tag of class mimeType. If not `nil`, the value of this property is the best available MIME type value for this type.

The value of this property is equivalent to, but more efficient than:

```
type.tags[.mimeType]?.first
```

## See Also

### Obtaining tags

var preferredFilenameExtension: String?

The preferred filename extension for the type.

var tags: [UTTagClass : [String]]

The tag specification dictionary of the type.

