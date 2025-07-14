

- Create ML Components
- ImageFeaturePrint
-  revision 

Instance Property

# revision

The feature extractor revision number.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var revision: Int { get set }
```

## Discussion

There are two Image Feature Print revisions: 1 and 2. In most cases revision 2 produces better models because it uses a smaller feature vector and better features.

In iOS 12 or later, tvOS 12 or later, and macOS 10.14 or later, revision 1 takes images with a size of 299x299 and produces a 2048 feature vector.

In iOS 17 or later, tvOS 17 or later, and macOS 14 or later, revision 2 takes images with a size of 360x360 and produces a 768 feature vector.

## See Also

### Getting the properties

let cropAndScale: VNImageCropAndScaleOption

The crop and scale options.

static let latestRevision: Int

The latest feature extractor revision.

