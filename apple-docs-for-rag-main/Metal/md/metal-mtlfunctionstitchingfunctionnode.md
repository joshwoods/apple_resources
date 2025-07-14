

- Metal
-  MTLFunctionStitchingFunctionNode 

Class

# MTLFunctionStitchingFunctionNode

A call graph node that describes a function call and its inputs.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MTLFunctionStitchingFunctionNode
```

## Overview

When the Metal device object evaluates the function graph to compile the stitched function, it evaluates the nodes stored in the arguments property that it hasn’t already evaluated, and then calls the function specified by name to generate the node’s output.

If the function has side effects on the input data, use the controlDependencies property on other nodes to specify whether the Metal device object must evaluate this node first.

## Topics

### Initializing a Function Node

init(name: String, arguments: [any MTLFunctionStitchingNode], controlDependencies: [MTLFunctionStitchingFunctionNode])

Creates a new function node.

### Configuring a Function Node

var name: String

The name of the function to call.

var arguments: [any MTLFunctionStitchingNode]

An ordered list of the nodes that provide the function’s arguments.

var controlDependencies: [MTLFunctionStitchingFunctionNode]

The list of nodes that must execute before executing the node.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MTLFunctionStitchingNode
- NSCopying
- NSObjectProtocol

## See Also

### Stitched Function Libraries

Customizing shaders using function pointers and stitching

Define custom shader behavior at runtime by creating functions from existing ones and preferentially linking to others in a dynamic library.

class MTLStitchedLibraryDescriptor

A description of a new library of procedurally generated functions.

class MTLFunctionStitchingGraph

A description of a new stitched function.

class MTLFunctionStitchingInputNode

A call graph node that describes an input to the call graph.

protocol MTLFunctionStitchingNode

A protocol to identify call graph nodes.

class MTLFunctionStitchingAttributeAlwaysInline

An attribute to specify that Metal needs to inline all of the function calls when generating the stitched function.

protocol MTLFunctionStitchingAttribute

A protocol to identify types that customize how the Metal compiler stitches a function together.

