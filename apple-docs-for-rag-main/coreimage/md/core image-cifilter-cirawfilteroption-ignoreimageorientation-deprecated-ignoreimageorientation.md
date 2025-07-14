

- Core Image
- CIFilter
- CIRAWFilterOption
-  ignoreImageOrientation Deprecated

Type Property

# ignoreImageOrientation

A key for specifying whether to ignore the image orientation. The associated value is a Boolean value packaged as an NSNumber object. The default value is `false`. An image is usually loaded in its proper orientation, as long as the associated metadata records its orientation. For special purposes you might want to load the image in its physical orientation. The exact meaning of "physical orientation” is dependent on the specific image.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let ignoreImageOrientation: CIRAWFilterOption
```

