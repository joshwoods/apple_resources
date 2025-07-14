

- Metal
-  MTLStitchedLibraryDescriptor 

Class

# MTLStitchedLibraryDescriptor

A description of a new library of procedurally generated functions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MTLStitchedLibraryDescriptor
```

## Overview

An MTLStitchedLibraryDescriptor describes a library of new stitched functions. A *stitched function* is a visible function you create by composing other Metal shader functions together in a function graph.

Configure a stitched library descriptor by assigning an array of one or more MTLFunctionStitchingGraph instances, each describing a stitched function, to the functionGraphs property. Then assign an MTLFunction array that includes all the functions the graphs depend on to the functions property.

Create a stitched library from the descriptor by passing it to the makeLibrary(stitchedDescriptor:) method of an MTLDevice. You can change the descriptor to create other libraries without affecting any existing ones.

## Topics

### Configuring a Stitched Library

var functions: [any MTLFunction]

The list of functions for creating the stitched library.

var functionGraphs: [MTLFunctionStitchingGraph]

The function graphs that define the new stitched library’s functions.

### Instance Properties

var binaryArchives: [any MTLBinaryArchive]

var options: MTLStitchedLibraryOptions

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Stitched Function Libraries

Customizing shaders using function pointers and stitching

Define custom shader behavior at runtime by creating functions from existing ones and preferentially linking to others in a dynamic library.

class MTLFunctionStitchingGraph

A description of a new stitched function.

class MTLFunctionStitchingInputNode

A call graph node that describes an input to the call graph.

class MTLFunctionStitchingFunctionNode

A call graph node that describes a function call and its inputs.

protocol MTLFunctionStitchingNode

A protocol to identify call graph nodes.

class MTLFunctionStitchingAttributeAlwaysInline

An attribute to specify that Metal needs to inline all of the function calls when generating the stitched function.

protocol MTLFunctionStitchingAttribute

A protocol to identify types that customize how the Metal compiler stitches a function together.

