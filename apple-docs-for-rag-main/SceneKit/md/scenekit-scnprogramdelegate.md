

- SceneKit
-  SCNProgramDelegate 

Protocol

# SCNProgramDelegate

The interface for tracking errors that occur when compiling shader source code.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
protocol SCNProgramDelegate : NSObjectProtocol
```

## Overview

You create and use custom shader programs with the SCNProgram class.

## Topics

### Handling Shader Compilation Errors

func program(SCNProgram, handleError: any Error)

Tells the delegate that an error occurred when compiling GLSL source code.

let SCNErrorDomain: String

Identifies an error type defined by the SceneKit framework.

SceneKit Error Codes

### Finding Fragment Opaqueness

func programIsOpaque(SCNProgram) -> Bool

Asks the delegate whether fragments rendered by a program are opaque.

Deprecated

### Binding and Unbinding Values

func program(SCNProgram, bindValueForSymbol: String, atLocation: UInt32, programID: UInt32, renderer: SCNRenderer) -> Bool

Invoked on the delegate to let it bind program values and/or associated graphics resources (such as textures) for symbols.

Deprecated

func program(SCNProgram, unbindValueForSymbol: String, atLocation: UInt32, programID: UInt32, renderer: SCNRenderer)

Invoked on the delegate to let it unbind program values and/or also unbind associated graphic resources (such as textures).

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing a Delegate Object

var delegate: (any SCNProgramDelegate)?

The delegate of the program object.

