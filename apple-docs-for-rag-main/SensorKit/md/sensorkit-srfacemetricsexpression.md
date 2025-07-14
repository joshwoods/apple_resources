

- SensorKit
-  SRFaceMetricsExpression 

Class

# SRFaceMetricsExpression

An object that represents a facial expression.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRFaceMetricsExpression
```

## Overview

Use the identifier property to determine the facial expression.

## Topics

### Getting the expression identifier and analysis

var value: Double

The current position of the expression.

var identifier: String

An identifier for the facial expression.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Getting face analytics

var faceAnchor: ARFaceAnchor

The anchor for the face that the sensor detects in front of the camera.

var partialFaceExpressions: [SRFaceMetricsExpression]

The partial face expressions that the algorithm detects.

var wholeFaceExpressions: [SRFaceMetricsExpression]

The whole face expressions that the algorithm detects.

