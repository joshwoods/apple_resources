

- Core Image
- Reduction Filters
-  areaMinimum() 

Type Method

# areaMinimum()

Calculates the minimum color component values for a specified area of the image.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func areaMinimum() -> any CIFilter & CIAreaMinimum
```

## Return Value

A 1 x 1 size image containing the minimum color component values.

## Discussion

This filter returns the minimum color components in the region defined by `extent`.

The area minimum filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`extent`  
A CGRect that specifies the subregion of the image that you want to process.

The following code creates a filter that calculates the minimum color components of a 500 x 500 set of pixels from the center of the image:

func areaMinimum(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.areaMinimum()
    filter.inputImage = inputImage
    filter.extent = CGRect(
        x: inputImage.extent.width/2-250,
        y: inputImage.extent.height/2-250,
        width: 500,
        height: 500)
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

