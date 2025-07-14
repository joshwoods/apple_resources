

- Core Image
- Reduction Filters
-  kMeans() 

Type Method

# kMeans()

Applies the k-means algorithm to find the most common colors in an image.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func kMeans() -> any CIFilter & CIKMeans
```

## Return Value

A one-dimensional CIImage containing the colors.

## Discussion

This filter uses the k-means clustering algorithm to find the most common colors in an input image. The result is a `CIImage` with `count` x 1 dimensions. Each `RGBA` pixel in the result image represents the center of a k-means cluster. The `RGB` components contain the color and the alpha component represents the weight of the color. You typically use the kMeans() filter in conjunction with the palettize() filter to produce an image with a reduced number of colors.

`inputImage`  
A `CIImage` to process.

`extent`  
A CGRect specifying the area of the image to analyze.

`means`  
An optional CIImage containing a set of colors to use as seeds for the k-means clustering.

`count`  
The number of k-means color clusters that should be created. Maximum is `128`, and default is `8`.

`passes`  
The number of k-means passes that should run. Maximum is `20`, and default is `5`.

`perceptual`  
Whether the k-means color palette should use a perceptual color space.

Tip

The colors in the result of the `kMeans()` filter have an alpha component that indicates the weight of the color. You should set this value one using settingAlphaOne(in:) before using the palette.

The following code example uses the `kMeans()` filter followed by the `palettize()` filter to reduce the colors in the image to four:

func kMeans(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.kMeans()
    filter.inputImage = inputImage
    filter.extent = inputImage.extent
    filter.count = 4
    filter.passes = 5
    return filter.outputImage!
}

func palettize(inputImage: CIImage, paletteImage: CIImage) -> CIImage {
    let palettize = CIFilter.palettize()
    palettize.inputImage = inputImage
    palettize.paletteImage = paletteImage
    return palettize.outputImage!
}

let palette = kMeans(inputImage: image)
let palettized = palettize(inputImage: image, palette.settingAlphaOne(in: palette.extent))

## See Also

### Filters

class func areaAverage() -> any CIFilter &amp; CIAreaAverage

Returns a 1 x 1 pixel image that contains the average color for the region of interest.

class func areaHistogram() -> any CIFilter &amp; CIAreaHistogram

Returns a histogram of a specified area of the image.

class func areaLogarithmicHistogram() -> any CIFilter &amp; CIAreaLogarithmicHistogram

Returns a logarithmic histogram of a specified area of the image.

class func areaMaximum() -> any CIFilter &amp; CIAreaMaximum

Calculates the maximum color components of a specified area of the image.

class func areaMaximumAlpha() -> any CIFilter &amp; CIAreaMaximumAlpha

Finds the pixel with the highest alpha value.

class func areaMinimum() -> any CIFilter &amp; CIAreaMinimum

Calculates the minimum color component values for a specified area of the image.

class func areaMinimumAlpha() -> any CIFilter &amp; CIAreaMinimumAlpha

Calculates the pixel within a specified area that has the smallest alpha value.

class func areaMinMax() -> any CIFilter &amp; CIAreaMinMax

Calculates minimum and maximum color components for a specified area of the image.

class func areaMinMaxRed() -> any CIFilter &amp; CIAreaMinMaxRed

Calculates the minimum and maximum red component value.

class func columnAverage() -> any CIFilter &amp; CIColumnAverage

Calculates the average color for a specified column of an image.

class func histogramDisplay() -> any CIFilter &amp; CIHistogramDisplay

Generates a histogram map from the image.

class func rowAverage() -> any CIFilter &amp; CIRowAverage

Calculates the average color for the specified row of pixels in an image.

