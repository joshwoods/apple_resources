

- SensorKit
- SRFaceMetrics
-  SRFaceMetrics.Context 

Structure

# SRFaceMetrics.Context

The context of the system during the camera session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Context
```

## Topics

### Camera contexts

static var deviceUnlock: SRFaceMetrics.Context

The camera session occurs while the user has the device unlocked.

static var messagingAppUsage: SRFaceMetrics.Context

The camera session occurs while the user is in the app with messaging capability.

### Creating camera contexts

init(rawValue: UInt)

Creates and returns a new structure with the specified value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting session information

var sessionIdentifier: String

An identifier for the camera session.

var context: SRFaceMetrics.Context

The context of the system during the camera session.

var version: String

The version of the algorithm that the system uses to generate the face metrics and analytics.

