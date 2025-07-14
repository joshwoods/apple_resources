

- Core Graphics
-  CGPatternCallbacks 

Structure

# CGPatternCallbacks

A structure that holds a version and two callback functions for drawing a custom pattern.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGPatternCallbacks
```

## Overview

You supply a CGPatternCallbacks structure to the function init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:) to create a data provider for direct access. The functions specified by the CGPatternCallbacks structure are responsible for drawing the pattern and for handling the pattern’s memory management.

## Topics

### Initializers

init()

init(version: UInt32, drawPattern: CGPatternDrawPatternCallback?, releaseInfo: CGPatternReleaseInfoCallback?)

### Instance Properties

var drawPattern: CGPatternDrawPatternCallback?

A pointer to a custom function that draws thepattern. For information about this callback function, see CGPatternDrawPatternCallback.

var releaseInfo: CGPatternReleaseInfoCallback?

An optional pointer to a custom function that’sinvoked when the pattern is released. CGPatternReleaseInfoCallback.

var version: UInt32

The version of the structure passed in as a parameterto the init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:). Forthis version of the structure, you should set this value to zero.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Callbacks

typealias CGPatternDrawPatternCallback

Draws a pattern cell.

typealias CGPatternReleaseInfoCallback

Release private data or resources associated with the pattern.

