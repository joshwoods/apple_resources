

- SceneKit
-  SCNColorMask 

Structure

# SCNColorMask

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
struct SCNColorMask
```

## Topics

### Initializers

init(rawValue: Int)

### Type Properties

static var all: SCNColorMask

static var alpha: SCNColorMask

static var blue: SCNColorMask

static var green: SCNColorMask

static var red: SCNColorMask

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

### Managing Render Targets

var writesToDepthBuffer: Bool

A Boolean value that determines whether SceneKit produces depth information when rendering the material.

var readsFromDepthBuffer: Bool

A Boolean value that determines whether SceneKit uses depth information when rendering the material.

var colorBufferWriteMask: SCNColorMask

