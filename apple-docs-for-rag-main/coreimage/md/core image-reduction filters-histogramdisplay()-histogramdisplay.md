

- Core Image
- Reduction Filters
-  histogramDisplay() 

Type Method

# histogramDisplay()

Generates a histogram map from the image.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func histogramDisplay() -> any CIFilter & CIHistogramDisplay
```

## Return Value

The generated image.

## Discussion

This method applies the histogram display filter to the result of the output from the areaHistogram() filter. This effect shows a graphical representation of the tonal distribution of colors in the image.

The histogram display filter uses the following properties:

`inputImage`  
An image with the type CIImage. Typically this is the output from the area histogram filter.

`height`  
A `float` representing the height of the generated histogram image as an NSNumber.

`lowLimit`  
A `float` representing the fraction of the left portion of the histogram image to make darker as an `NSNumber`.

`hightLimit`  
A `float` representing the fraction of the right portion of the histogram to make lighter as an `NSNumber`.

The following code creates a filter that results in a histogram diagram generated from the input image:

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

class func kMeans() -> any CIFilter &amp; CIKMeans

Applies the k-means algorithm to find the most common colors in an image.

class func rowAverage() -> any CIFilter &amp; CIRowAverage

Calculates the average color for the specified row of pixels in an image.

