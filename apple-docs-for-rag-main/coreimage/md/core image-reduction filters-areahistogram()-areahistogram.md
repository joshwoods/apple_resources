

- Core Image
- Reduction Filters
-  areaHistogram() 

Type Method

# areaHistogram()

Returns a histogram of a specified area of the image.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func areaHistogram() -> any CIFilter & CIAreaHistogram
```

## Return Value

A 1 pixel high image containing the calculated histogram`.`

## Discussion

This filter calculates histograms of the red, green, blue, and alpha colors in the region defined by `extent`. The `count` property controls the number of bins (or width) of the histogram. The filter scales the histogram so that the total of all the counts in the bins equals `scale`.

The area histogram filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`extent`  
A CGRect that specifies the subregion of the image that you want to process.

`scale`  
The scale value to use for the histogram values. If the scale is 1, then the total of all the counts in the histogram equals 1.

`count`  
The number of bins for the histogram. This value determines the width of the output image. Minimum value 1, maximum value 2048.

The following code creates a filter that results in an image that has a height of 1 pixel and a width of 256 pixels. The pixel color components contain the histogram values.

func areaHistogram(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.areaHistogram()
    filter.inputImage = inputImage
    filter.count = 256
    filter.scale = 50
    filter.extent = CGRect(
        x: inputImage.extent.width/2-250,
        y: inputImage.extent.height/2-250,
        width: 500,
        height: 500)
    return filter.outputImage!
}

To display the histogram, you can use the histogramDisplay() filter:

func histogramDisplay(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.histogramDisplay()
    filter.inputImage = areaHistogram(inputImage: inputImage)
    filter.highLimit = 1
    filter.height = 100
    filter.lowLimit = 0
    return filter.outputImage!
}

## See Also

### Filters

class func areaAverage() -> any CIFilter &amp; CIAreaAverage

Returns a 1 x 1 pixel image that contains the average color for the region of interest.

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

class func kMeans() -> any CIFilter &amp; CIKMeans

Applies the k-means algorithm to find the most common colors in an image.

class func rowAverage() -> any CIFilter &amp; CIRowAverage

Calculates the average color for the specified row of pixels in an image.

