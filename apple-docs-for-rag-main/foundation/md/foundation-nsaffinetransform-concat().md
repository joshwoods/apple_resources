

- Foundation
- NSAffineTransform
-  concat() 

Instance Method

# concat()

Appends the receiver’s matrix to the current transformation matrix stored in the current graphics context, replacing the current transformation matrix with the result.

macOS 10.0+

``` source
func concat()
```

## Discussion

Concatenation is performed by matrix multiplication—see Manipulating Transform Values.

If this method is invoked from within an `NSView`draw(_:) method, then the current transformation matrix is an accumulation of the screen, window, and any superview’s transformation matrices. Invoking this method defines a new user coordinate system whose coordinates are mapped into the former coordinate system according to the receiver’s transformation matrix. To undo the concatenation, you must invert the receiver’s matrix and invoke this method again.

## See Also

### Related Documentation

func invert()

Replaces the receiver’s matrix with its inverse matrix.

### Setting and Building the Current Transformation Matrix

func set()

Sets the current transformation matrix to the receiver’s transformation matrix.

