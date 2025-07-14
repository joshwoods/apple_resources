

- Core ML
- MLMultiArray
-  init(shape:dataType:) 

Initializer

# init(shape:dataType:)

Creates a multidimensional array with a shape and type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    shape: [NSNumber],
    dataType: MLMultiArrayDataType
) throws
```

## Parameters 

`shape`  

An integer array that has an element for each dimension in a multiarray that represents its length.

`dataType`  

An element type defined by MLMultiArrayDataType.

## Discussion

This method allocates a contiguous region of memory for the multiarray’s shape. You must set the contents of memory. The multiarray frees the memory in its deinitializer (Swift) or dealloc method (Objective-C).

The following code creates a 3 x 3 multiarray and sets its contents to the value 3.14159.

- Swift
- Objective-C

```
// Create a 2D multiarray with dimension 3 x 3.
let shape3x3 = [3, 3] as [NSNumber]

guard let multiarray3x3 = try? MLMultiArray(shape: shape3x3, dataType: .float) else {
    // Handle the error.
    return
}

print("Before: \(multiarray3x3)")

// Initialize the multiarray.
for xCoordinate in 0..

```
NSError *error = nil;

// Create a 2D multiarray with dimension 3 x 3.
NSArray *shape3x3 = @[@3, @3];

MLMultiArray *multiarray3x3 = [[MLMultiArray alloc] initWithShape:shape3x3 dataType:MLMultiArrayDataTypeFloat error: &error];
if (error != nil) {
    // Handle the error.
    return;
}

NSLog(@"Before: %@\n", multiarray3x3);

// Initialize the multiarray.
for (int x = 0; x 

## See Also

### Creating a Multiarray

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of integers.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of floats.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of doubles.

convenience init&lt;ShapedArray>(ShapedArray)

Creates a multiarray from a shaped array.

init(dataPointer: UnsafeMutableRawPointer, shape: [NSNumber], dataType: MLMultiArrayDataType, strides: [NSNumber], deallocator: ((UnsafeMutableRawPointer) -> Void)?) throws

Creates a multiarray from a data pointer.

convenience init(byConcatenatingMultiArrays: [MLMultiArray], alongAxis: Int, dataType: MLMultiArrayDataType)

Merges an array of multiarrays into one multiarray along an axis.

init(pixelBuffer: CVPixelBuffer, shape: [NSNumber])

Creates a multiarray sharing the surface of a pixel buffer.

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

