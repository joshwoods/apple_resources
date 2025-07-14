

- SensorKit
-  SRFaceMetrics 

Class

# SRFaceMetrics

An object that represents metrics about the user’s face.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRFaceMetrics
```

## Overview

The faceMetrics sensor provides this class as its sample type.

## Topics

### Getting session information

var sessionIdentifier: String

An identifier for the camera session.

var context: SRFaceMetrics.Context

The context of the system during the camera session.

struct Context

The context of the system during the camera session.

var version: String

The version of the algorithm that the system uses to generate the face metrics and analytics.

### Getting face analytics

var faceAnchor: ARFaceAnchor

The anchor for the face that the sensor detects in front of the camera.

var partialFaceExpressions: [SRFaceMetricsExpression]

The partial face expressions that the algorithm detects.

var wholeFaceExpressions: [SRFaceMetricsExpression]

The whole face expressions that the algorithm detects.

class SRFaceMetricsExpression

An object that represents a facial expression.

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

### Analyzing faces

var SR_ARKIT_SUPPORTED: Int32

A flag that indicates whether the ARKit framework is available in the SDK for the SensorKit framework.

