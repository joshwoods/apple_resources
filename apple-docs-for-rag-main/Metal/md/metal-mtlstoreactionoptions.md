

- Metal
-  MTLStoreActionOptions 

Structure

# MTLStoreActionOptions

Options that modify a store action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct MTLStoreActionOptions
```

## Overview

This property modifies the intended behavior of the store actions in the MTLStoreAction enumeration.

## Topics

### Constants

init(rawValue: UInt)

Creates a store action option from a raw integer value.

static var customSamplePositions: MTLStoreActionOptions

An option that stores data in a sample-position–agnostic representation.

### Using Programmable Sample Positions

static var customSamplePositions: MTLStoreActionOptions

An option that stores data in a sample-position–agnostic representation.

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

### Encoding a Render Pass in Parallel

protocol MTLParallelRenderCommandEncoder

An object that splits up a single render pass so that it can be simultaneously encoded from multiple threads.

enum MTLLoadAction

Types of actions performed for an attachment at the start of a rendering pass.

enum MTLStoreAction

Types of actions performed for an attachment at the end of a rendering pass.

