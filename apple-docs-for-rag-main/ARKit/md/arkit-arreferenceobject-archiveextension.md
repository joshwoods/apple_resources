

- ARKit
- ARReferenceObject
-  archiveExtension 

Type Property

# archiveExtension

The standard filename extension for exported ARReferenceObject instances.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class let archiveExtension: String
```

## Discussion

Use this filename extension when constructing a URL to save a reference object file with the export(to:previewImage:) method.

## See Also

### Saving Recorded Objects

func export(to: URL, previewImage: UIImage?) throws

Writes a binary representation of the object to the specified file URL.

