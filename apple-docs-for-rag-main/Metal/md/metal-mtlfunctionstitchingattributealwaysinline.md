

- Metal
-  MTLFunctionStitchingAttributeAlwaysInline 

Class

# MTLFunctionStitchingAttributeAlwaysInline

An attribute to specify that Metal needs to inline all of the function calls when generating the stitched function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MTLFunctionStitchingAttributeAlwaysInline
```

## Overview

To inline functions in a call graph, instantiate an instance of this class and assign it as an attribute on the MTLFunctionStitchingGraph.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MTLFunctionStitchingAttribute
- NSObjectProtocol

## See Also

### Related Documentation

var attributes: [any MTLFunctionStitchingAttribute]

A list of attributes to configure how the Metal device object generates the new stitched function.

### Stitched Function Libraries

Customizing shaders using function pointers and stitching

Define custom shader behavior at runtime by creating functions from existing ones and preferentially linking to others in a dynamic library.

class MTLStitchedLibraryDescriptor

A description of a new library of procedurally generated functions.

class MTLFunctionStitchingGraph

A description of a new stitched function.

class MTLFunctionStitchingInputNode

A call graph node that describes an input to the call graph.

class MTLFunctionStitchingFunctionNode

A call graph node that describes a function call and its inputs.

protocol MTLFunctionStitchingNode

A protocol to identify call graph nodes.

protocol MTLFunctionStitchingAttribute

A protocol to identify types that customize how the Metal compiler stitches a function together.

