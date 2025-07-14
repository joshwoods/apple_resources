

- Metal
-  MTLIntersectionFunctionSignature 

Structure

# MTLIntersectionFunctionSignature

Constants for specifying different types of custom intersection functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLIntersectionFunctionSignature
```

## Overview

For more information on declaring intersection functions in MSL, see Metal Shading Language Specification.

## Topics

### Initializing the Intersection Function Signature

init(rawValue: UInt)

Returns a new signature description from a specified raw value.

### Specifying the Intersection Function Signature

static var instancing: MTLIntersectionFunctionSignature

A flag indicating that function signature uses instancing.

static var triangleData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses triangle data.

static var worldSpaceData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses world space data.

### Type Properties

static var curveData: MTLIntersectionFunctionSignature

static var extendedLimits: MTLIntersectionFunctionSignature

static var instanceMotion: MTLIntersectionFunctionSignature

static var maxLevels: MTLIntersectionFunctionSignature

static var primitiveMotion: MTLIntersectionFunctionSignature

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

### Intersection Function Tables

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

