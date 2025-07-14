

- Uniform Type Identifiers
- UTType
-  tags 

Instance Property

# tags

The tag specification dictionary of the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var tags: [UTTagClass : [String]] { get }
```

## Discussion

Uniform Type Identifiers don’t store tag information for nonstandard tag classes. Identifiers normalize string values into arrays that contain those strings. For example, a tag specification dictionary with values of:

```
{
    "public.mime-type": "x/y",
    "nonstandard-tag-class": "abc",
}
```

Normalizes to:

```
{
    "public.mime-type": ["x/y"]
}
```

Use the tag class mimeType or filenameExtension to retrieve the list of supporting MIME types or filename extensions for your type. For example, the following example retrieves a list of the filename extensions for the mpeg type:

```
let MPEGextensions = UTType.mpeg.tags[.filenameExtension]
```

Types that have no tags for the requested tag class return a nil, not an empty array.

To get the preferred filename extension or MIME type, use the tag class preferredFilenameExtension or preferredMIMEType, respectively.

## See Also

### Obtaining tags

var preferredFilenameExtension: String?

The preferred filename extension for the type.

var preferredMIMEType: String?

The preferred MIME type for the type.

