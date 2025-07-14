

- Accelerate
- BNNSGraph
-  BNNSGraph.Context 

Class

# BNNSGraph.Context

A wrapper around a compiled graph object that adds a required modifiable context to support dynamically sized models and set execute-time options.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
class Context
```

## Overview

A BNNSGraph.Context instance provides a wrapper around the C API bnns_graph_t and bnns_graph_context_t types. Because this class manages its own memory, you don’t need to call BNNSGraphContextDestroy(_:) to deallocate its resources.

## Topics

### Creating a graph context

init(compileFromPath: String, functionName: String?, options: BNNSGraph.CompileOptions) async throws

Returns a new context that wraps a graph object representing the compiled mlmodelc file.

struct CompileOptions

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

### Specifying and querying a graph context’s properties

func setBatchSize(Int, forFunction: String?) async

Sets the batch size for a graph.

func setDynamicShapes([BNNSGraph.Shape], forFunction: String?) async throws -> [BNNSGraph.Shape]

Specifies the dynamic shapes for a graph and, if possible, infers the output shapes.

struct Shape

The specification of the shape of an argument.

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

### Specifying a tensor’s properties

func tensor(forFunction: String?, argument: String, fillKnownDynamicShapes: Bool) -> BNNSTensor?

Returns an unallocated tensor for a given function argument.

### Executing a graph

func executeFunction(String?, arguments: inout [BNNSTensor]) async throws

Executes the specified function using an array of input and output tensors.

func executeFunction&lt;T>(String?, arguments: [T]) throws

Executes the specified function using an array of input and output pointers.

protocol PointerArgument

A type that BNNS Graph accepts as an input-output argument.

### Handling errors

enum Error

Error codes that a graph context throws.

