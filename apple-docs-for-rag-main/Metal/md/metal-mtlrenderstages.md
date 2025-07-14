

- Metal
-  MTLRenderStages 

Structure

# MTLRenderStages

The stages in a render pass that triggers a synchronization command.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
struct MTLRenderStages
```

## Overview

Render stage boundaries provide synchronization opportunities within a render pass for specific resources and resource types. For example, you can designate render stage a synchronization point for a memory barrier or a fence (see memoryBarrier(resources:after:before:) and MTLFence, respectively). This allows a GPU to overlap its execution of two adjacent stages, which can shorten its overall runtime for the render pass.

## Topics

### Render Pass Stages

static var object: MTLRenderStages

The object rendering stage.

static var mesh: MTLRenderStages

The mesh rendering stage.

static var vertex: MTLRenderStages

The vertex rendering stage.

static var fragment: MTLRenderStages

The fragment rendering stage.

static var tile: MTLRenderStages

The tile rendering stage.

### Swift Support

init(rawValue: UInt)

Creates a render stage from a raw value.

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

### Synchronization

Synchronizing CPU and GPU Work

Avoid stalls between CPU and GPU work by using multiple instances of a resource.

