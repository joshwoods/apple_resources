

- Core Image
- Reduction Filters
-  areaLogarithmicHistogram() 

Type Method

# areaLogarithmicHistogram()

Returns a logarithmic histogram of a specified area of the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.5+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func areaLogarithmicHistogram() -> any CIFilter & CIAreaLogarithmicHistogram
```

## Return Value

A 1-pixel-high image containing the calculated histogram`.`

## Discussion

This filter calculates histograms of the `red,``green,``blue,` and `alpha` colors for the specified area of an image. A base two-logarithm function is applied to the values before binning. The `count` property controls the number of bins (or width) of the histogram. The histogram is scaled so that all the values sum to `scale`.

`inputImage`  
An image with the type CIImage.

`extent`  
A CGRect that specifies the subregion of the image you want to process.

`scale`  
The scale value for the histogram values. If the scale is `1`, then the bins in the resulting image sum to `1`.

`count`  
The number of bins for the histogram. This value determines the width of the output image. Minimum value `1`, and maximum value `2048`.

`minimumStop`  
The minimum of the range of color channel values in the logarithmic histogram image. Defaults to `-10`.

`maximumStop`  
The maximum of the range of color channel values in the logarithmic histogram image. Defaults to 4.

The following code creates a filter that results in a 1-pixel-tall image with a width of 256. The pixel color components contain the logarithmic histogram values:

func areaLogarithmicHistogram(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.areaLogarithmicHistogram()
    filter.inputImage = inputImage
    filter.count = 256
    filter.scale = 15
    filter.extent = CGRect(
        x: inputImage.extent.width/2-250,
        y: inputImage.extent.height/2-250,
        width: 500,
        height: 500)
    return filter.outputImage!
}

Use the histogramDisplay() filter to display the histogram:

func logarithmicHistogramDisplay(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.histogramDisplay()
    filter.inputImage = areaLogarithmicHistogram(inputImage: inputImage)
    filter.highLimit = 1
    filter.height = 100
    filter.lowLimit = 0
    return filter.outputImage!
}

## See Also

### Filters

class func areaAverage() -> any CIFilter &amp; CIAreaAverage

Returns a 1 x 1 pixel image that contains the average color for the region of interest.

class func areaHistogram() -> any CIFilter &amp; CIAreaHistogram

Returns a histogram of a specified area of the image.

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

class func kMeans() -> any CIFilter &amp; CIKMeans

Applies the k-means algorithm to find the most common colors in an image.

class func rowAverage() -> any CIFilter &amp; CIRowAverage

Calculates the average color for the specified row of pixels in an image.

