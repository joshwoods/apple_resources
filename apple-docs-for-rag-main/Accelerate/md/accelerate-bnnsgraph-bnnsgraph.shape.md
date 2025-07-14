

- Accelerate
- BNNSGraph
-  BNNSGraph.Shape 

Structure

# BNNSGraph.Shape

The specification of the shape of an argument.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
struct Shape
```

## Overview

The setDynamicShapes(_:forFunction:) function uses arrays of BNNSGraph.Shape structures as its input and output. This structure wraps the C API bnns_graph_shape_t type and derives its rank from the number of elements in the dimensions array.

## Topics

### Creating a shape structure

init(arrayLiteral: Int...)

Creates a shape structure from the given array literal.

init([Int])

Creates a shape structure from the given array elements.

### Querying a shape structure’s properties

var dimensions: [Int]

An array that contains the dimensions of the shape structure.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

## Relationships

### Conforms To

- ExpressibleByArrayLiteral

## See Also

### Specifying and querying a graph context’s properties

func setBatchSize(Int, forFunction: String?) async

Sets the batch size for a graph.

func setDynamicShapes([BNNSGraph.Shape], forFunction: String?) async throws -> [BNNSGraph.Shape]

Specifies the dynamic shapes for a graph and, if possible, infers the output shapes.

func argumentCount(forFunction: String?) -> Int

Returns the number of arguments for the given function argument.

func argumentNames(forFunction: String?) -> [String]

Returns the names of arguments for the given function argument.

func argumentPosition(forFunction: String?, argument: String) -> Int

Returns the index into the arguments array for the given function argument.

var functionCount: Int

The number of input arguments for the given function argument.

var functionNames: [String]

Returns the names of callable functions in the graph.

var checkForNaNsAndInfinities: Bool

A Boolean value that specifies that the context checks intermediate tensors for NaNs and infinities.

