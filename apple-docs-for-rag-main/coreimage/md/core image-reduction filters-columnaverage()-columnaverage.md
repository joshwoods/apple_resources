

- Core Image
- Reduction Filters
-  columnAverage() 

Type Method

# columnAverage()

Calculates the average color for a specified column of an image.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func columnAverage() -> any CIFilter & CIColumnAverage
```

## Return Value

The generated image.

## Discussion

This method applies the column average filter to an image. This effect calculates the average color for a vertical column over a region defined by `extent`. The width of the resulting image is set by the width of the `extent`. The height of the resulting image is always 1 pixel.

The column average filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`extent`  
A CGRect that specifies the subregion of the image that you want to process.

The following code creates an image containing the average values in the columns from the middle of the image:

func columnAverage(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.columnAverage()
    filter.inputImage = inputImage
    filter.extent = CGRect(x: 0, y: inputImage.extent.height/3, width: inputImage.extent.width, height: inputImage.extent.height/3)
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

class func histogramDisplay() -> any CIFilter &amp; CIHistogramDisplay

Generates a histogram map from the image.

class func kMeans() -> any CIFilter &amp; CIKMeans

Applies the k-means algorithm to find the most common colors in an image.

class func rowAverage() -> any CIFilter &amp; CIRowAverage

Calculates the average color for the specified row of pixels in an image.

