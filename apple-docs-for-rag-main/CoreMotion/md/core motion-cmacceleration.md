

- Core Motion
-  CMAcceleration 

Structure

# CMAcceleration

The type of a structure containing 3-axis acceleration values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMAcceleration
```

## Overview

A G is a unit of gravitation force equal to that exerted by the earth’s gravitational field (9.81 m s−2).

## Topics

### Initializers

init()

init(x: Double, y: Double, z: Double)

### Getting the Acceleration Values

var x: Double

X-axis acceleration in G’s (gravitational force).

var y: Double

Y-axis acceleration in G’s (gravitational force).

var z: Double

Z-axis acceleration in G’s (gravitational force).

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing Accelerometer Data

var acceleration: CMAcceleration

The acceleration measured by the accelerometer.

