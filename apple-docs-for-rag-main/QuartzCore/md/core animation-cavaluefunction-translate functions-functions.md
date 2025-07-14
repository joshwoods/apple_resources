

- Core Animation
- CAValueFunction
-  Translate Functions 

API Collection

# Translate Functions

Translate value transform functions construct a 4x4 matrix that represents the corresponding translate matrix.

## Topics

### Constants

static let translate: CAValueFunctionName

A value function that translates by the input values along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) translate values.

static let translateX: CAValueFunctionName

A value function translates by the input value along the x-axis. Animations referencing this value function must provide a single input value.

static let translateY: CAValueFunctionName

A value function translates by the input value along the y-axis. Animations referencing this value function must provide a single input value.

static let translateZ: CAValueFunctionName

A value function translates by the input value along the z-axis. Animations referencing this value function must provide a single input value.

## See Also

### Constants

Rotate Value Functions

Rotate value transform functions construct a 4x4 matrix that represents the corresponding rotation matrix.

Scale Value Functions

Scale value transform functions construct a 4x4 matrix that represents the corresponding scale matrix.

