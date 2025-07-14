

- Metal
-  MTLResourceUsage 

Structure

# MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct MTLResourceUsage
```

## Mentioned in 

Tracking the Resource Residency of Argument Buffers

## Overview

You can combine multiple MTLResourceUsage values with a bitwise OR (`|`) if the resource serves multiple purposes over its lifetime. You can enable options for certain resources that indicate whether the Metal driver needs to convert the resource to another format, such as whether it needs to decompress a color render target.

## Topics

### Initializers

init(rawValue: UInt)

Creates a set of resource options from a raw value.

### Type Properties

static var read: MTLResourceUsage

An option that enables reading from the resource.

static var write: MTLResourceUsage

An option that enables writing to the resource.

static var sample: MTLResourceUsage

An option that enables sampling from the resource.

Deprecated

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

### Common Resource Functionality

protocol MTLAllocation

A memory allocation from a Metal GPU device, such as a memory heap, texture, or data buffer.

protocol MTLResource

An allocation of memory accessible to a GPU.

struct MTLResourceOptions

Optional arguments used to set the behavior of a resource.

struct MTLResourceID

