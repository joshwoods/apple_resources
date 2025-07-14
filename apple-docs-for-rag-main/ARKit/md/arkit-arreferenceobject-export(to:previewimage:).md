

- ARKit
- ARReferenceObject
-  export(to:previewImage:) 

Instance Method

# export(to:previewImage:)

Writes a binary representation of the object to the specified file URL.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func export(
    to url: URL,
    previewImage: UIImage?
) throws
```

## Parameters 

`url`  

The file URL at which to write the reference object data.

`previewImage`  

A thumbnail image to be embedded in the reference object’s filesystem representation.

ARKit ignores preview images when loading reference objects. Instead, this image helps make reference object files visually identifiable in external tools like Xcode, Finder, and Quick Look.

## Discussion

After exporting a reference object from your object-scanning app to a file, you can bundle that reference object into other apps you create by inserting it into an Xcode asset catalog.

## See Also

### Saving Recorded Objects

class let archiveExtension: String

The standard filename extension for exported ARReferenceObject instances.

