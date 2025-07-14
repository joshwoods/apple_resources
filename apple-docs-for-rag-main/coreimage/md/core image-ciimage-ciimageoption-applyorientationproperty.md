

- Core Image
- CIImage
- CIImageOption
-  applyOrientationProperty 

Type Property

# applyOrientationProperty

The key for transforming an image according to orientation metadata.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let applyOrientationProperty: CIImageOption
```

## Discussion

Images can contain metadata that reveals the orientation at capture time. You can load this metadata into CIImage with imageWithContentsOfURL: or init(data:) when the captured image contains orientation metadata. Use any of the `initWith:options: `methods if the properties (NSDictionary of metadata properties) option is also provided.

If the value of this key is true, then calls to imageWithContentsOfURL:options: and imageWithData:options: will return the image transformed according to its orientation metadata.

