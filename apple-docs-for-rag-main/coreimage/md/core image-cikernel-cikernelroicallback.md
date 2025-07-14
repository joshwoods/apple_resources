

- Core Image
- CIKernel
-  CIKernelROICallback 

Type Alias

# CIKernelROICallback

The signature for a block that computes the region of interest (ROI) for a given area of destination image pixels. Core Image calls this block when applying the kernel. You specify this block when using the apply(extent:roiCallback:arguments:) method.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
typealias CIKernelROICallback = (Int32, CGRect) -> CGRect
```

## Discussion

The block takes the following parameters:

index  
For a general-purpose kernel or color kernel routine that supports multiple input images, the index of the source image for which Core Image is requesting ROI information. For all other kernel routines, this parameter is always zero.

rect  
The rectangle in destination image pixels for which Core Image is requesting ROI information.

The block returns a CGRect structure describing the region of interest for the specified rectangle.

When applying a filter kernel, the region of interest is the area of source image pixels that must be processed to produce a given area of destination image pixels. (For a more detailed definition, see The Region of Interest.) For example, a kernel that applies a blur effect in a ten-pixel radius must sample source image pixels ten pixels away in each direction from every output pixel. Thus, its region of interest is a rectangle ten pixels larger on each side than the destination rectangle:

CIKernelROICallback callback = ^(int index, CGRect rect) {
    return CGRectInset(rect, -10, -10);
};

If your kernel does not need the image at `index` to produce output in the rectangle `rect`, your block should return null.

## See Also

### Applying a Kernel to Filter an Image

func apply(extent: CGRect, roiCallback: CIKernelROICallback, arguments: [Any]) -> CIImage?

Creates a new image using the kernel and specified arguments.

