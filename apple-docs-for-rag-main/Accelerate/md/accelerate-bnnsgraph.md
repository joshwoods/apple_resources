

- Accelerate
-  BNNSGraph 

Enumeration

# BNNSGraph

An enumeration that acts as a namespace for the Swift overlays to BNNS Graph.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
enum BNNSGraph
```

## Topics

### Compiling a graph object and creating a context

class Context

A wrapper around a compiled graph object that adds a required modifiable context to support dynamically sized models and set execute-time options.

### Protocols

protocol PointerArgument

A type that BNNS Graph accepts as an input-output argument.

### Structures

struct CompileOptions

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

struct Shape

The specification of the shape of an argument.

### Enumerations

enum Error

Error codes that a graph context throws.

## See Also

### Enumerations

enum BNNS

An enumeration that acts as a namespace for Swift overlays to BNNS.

