

- Foundation
-  NSAffineTransform 

Class

# NSAffineTransform

A graphics coordinate transformation.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSAffineTransform
```

## Overview

In Swift, this object bridges to AffineTransform; use NSAffineTransform when you need reference semantics or other Foundation-specific behavior.

A transformation specifies how points in one coordinate system are transformed to points in another coordinate system. An affine transformation is a special type of transformation that preserves parallel lines in a path but does not necessarily preserve lengths or angles. Scaling, rotation, and translation are the most commonly used manipulations supported by affine transforms, but shearing is also possible.

Note

In OS X 10.3 and earlier the NSAffineTransform class was declared and implemented entirely in the Application Kit framework. As of macOS 10.4 the NSAffineTransform class has been split across the Foundation and Application Kit frameworks.

Methods for applying affine transformations to the current graphics context and a method for applying an affine transformation to an NSBezierPath object are described in NSAffineTransform Additions Reference in the Application Kit.

Important

The Swift overlay to the Foundation framework provides the AffineTransform structure, which bridges to the NSAffineTransform class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating an Affine Transform

init()

Initializes an affine transform matrix to the identity matrix.

convenience init(transform: NSAffineTransform)

Initializes the receiver’s matrix using another transform object.

### Accumulating Transformations

func rotate(byDegrees: Double)

Applies a rotation factor (measured in degrees) to the receiver’s transformation matrix.

func rotate(byRadians: Double)

Applies a rotation factor (measured in radians) to the receiver’s transformation matrix.

func scale(by: Double)

Applies the specified scaling factor along both x and y axes to the receiver’s transformation matrix.

func scaleX(by: Double, yBy: Double)

Applies scaling factors to each axis of the receiver’s transformation matrix.

func translateX(by: Double, yBy: Double)

Applies the specified translation factors to the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

### Transforming Data and Objects

func transform(NSPoint) -> NSPoint

Applies the receiver’s transform to the specified point and returns the result.

func transform(NSSize) -> NSSize

Applies the receiver’s transform to the specified size and returns the results.

func transform(NSBezierPath) -> NSBezierPath

Creates and returns a new NSBezierPath object with each point in the given path transformed by the receiver.

### Accessing the Transformation Matrix

var transformStruct: NSAffineTransformStruct

The matrix coefficients stored as the transformation matrix.

struct NSAffineTransformStruct

A structure that defines the three-by-three matrix that performs an affine transform between two coordinate systems.

### Setting and Building the Current Transformation Matrix

func set()

Sets the current transformation matrix to the receiver’s transformation matrix.

func concat()

Appends the receiver’s matrix to the current transformation matrix stored in the current graphics context, replacing the current transformation matrix with the result.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

