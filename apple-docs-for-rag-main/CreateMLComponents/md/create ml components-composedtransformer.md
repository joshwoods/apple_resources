

- Create ML Components
-  ComposedTransformer 

Structure

# ComposedTransformer

A transformer that composes two transformers by applying them one after the other.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ComposedTransformer where Inner : Transformer, Outer : Transformer, Inner.Output == Outer.Input
```

## Overview

The inner transformer’s output must match the outer transformer input. The result of this transformer is equivalent to invoking `outer(inner(x))` on an input `x`,

## Topics

### Creating the transformer

init(Inner, Outer)

Creates a transformer composition from two transformers.

### Getting the properties

var inner: Inner

The inner transformer.

var outer: Outer

The outer transformer.

### Performing the transformation

func applied(to: ComposedTransformer&lt;Inner, Outer>.Input, eventHandler: EventHandler?) async throws -> ComposedTransformer&lt;Inner, Outer>.Output

Performs the composed transformation on a single input.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Sendable
- Transformer

## See Also

### Composition

struct ComposedTemporalTransformer

A temporal transformer that composes two temporal transformers by applying them one after the other.

struct ComposedTabularTransformer

A transformer that composes two tabular transformers by applying them one after the other.

