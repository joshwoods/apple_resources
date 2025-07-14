

- SceneKit
-  SCNBillboardAxis 

Structure

# SCNBillboardAxis

Options for locking the orientation of nodes affected by a billboard constraint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SCNBillboardAxis
```

## Overview

The figure below shows the effects of constraining various axes.

## Topics

### Constants

static var X: SCNBillboardAxis

Align an affected node such that its x-axis is always parallel to that of the view, leaving it free to rotate otherwise.

static var Y: SCNBillboardAxis

Align an affected node such that its y-axis is always parallel to that of the view, leaving it free to rotate otherwise.

static var Z: SCNBillboardAxis

Align an affected node such that its z-axis is always perpendicular to the viewing plane, leaving it free to rotate otherwise.

static var all: SCNBillboardAxis

Align an affected node such that its orientation always matches that of the view.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

