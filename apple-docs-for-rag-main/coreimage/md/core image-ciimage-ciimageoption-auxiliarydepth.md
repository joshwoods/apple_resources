

- Core Image
- CIImage
- CIImageOption
-  auxiliaryDepth 

Type Property

# auxiliaryDepth

The key into the properties dictionary indicating whether to return an auxiliary depth image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let auxiliaryDepth: CIImageOption
```

## Discussion

The value of this key is an NSNumber containing a Boolean `true` or `false`. If the value is `true`, then calls to imageWithContentsOfURL:options: and imageWithData:options: will return the auxiliary image as a half-float monochrome image instead of the primary image, or `nil` if no auxiliary image exists.

