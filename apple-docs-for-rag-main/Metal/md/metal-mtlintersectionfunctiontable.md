

- Metal
-  MTLIntersectionFunctionTable 

Protocol

# MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIntersectionFunctionTable : MTLResource
```

## Overview

Don’t implement this protocol yourself. Instead create a MTLIntersectionFunctionTableDescriptor object and configure its properties. Then call the appropriate method on the pipeline state object that you want to use this table with:

Compute pipeline  
makeIntersectionFunctionTable(descriptor:)

Render pipeline  
makeIntersectionFunctionTable(descriptor:stage:)

If you use the same ray-tracing functions with more than one pipeline, make a separate table for each.

Use the methods on this object to set the table entries to point at the intersection functions, and to provide buffers as arguments for those functions. For more information about intersection functions, see Metal Shading Language Specification.

## Topics

### Setting a Table Entry

func setFunction((any MTLFunctionHandle)?, index: Int)

Sets an entry in the table.

**Required**

func setFunctions([(any MTLFunctionHandle)?], range: Range&lt;Int>)

Sets a range of entries in the table.

### Specifying Arguments for Intersection Functions

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Sets a buffer for the intersection functions.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Sets a range of buffers for the intersection functions.

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Sets a visible function table for the intersection functions.

**Required**

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Sets a range of visible function tables for the intersection functions.

### Specifying Opaque Triangle Intersection Testing

func setOpaqueTriangleIntersectionFunction(signature: MTLIntersectionFunctionSignature, index: Int)

Sets an entry in the intersection table to point to a system-defined opaque triangle intersection function.

**Required**

func setOpaqueTriangleIntersectionFunction(signature: MTLIntersectionFunctionSignature, range: NSRange)

Sets a range of entries in the intersection table to point to a system-defined opaque triangle intersection function.

**Required**

### Instance Properties

var gpuResourceID: MTLResourceID

**Required**

### Instance Methods

func setOpaqueCurveIntersectionFunction(signature: MTLIntersectionFunctionSignature, index: Int)

**Required**

func setOpaqueCurveIntersectionFunction(signature: MTLIntersectionFunctionSignature, range: NSRange)

**Required**

## Relationships

### Inherits From

- MTLAllocation
- MTLResource
- NSObjectProtocol

## See Also

### Intersection Function Tables

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

struct MTLIntersectionFunctionSignature

Constants for specifying different types of custom intersection functions.

