

- Create ML Components
-  ComposedTabularTransformer 

Structure

# ComposedTabularTransformer

A transformer that composes two tabular transformers by applying them one after the other.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ComposedTabularTransformer where Inner : TabularTransformer, Outer : TabularTransformer
```

## Overview

The result of this transformer is equivalent to invoking `outer(inner(x))` on an input `x`,

## Topics

### Creating the transformer

init(Inner, Outer)

Creates a composed tabular transformer from two tabular transformers.

### Getting the properties

var inner: Inner

The inner transformer.

var outer: Outer

The outer transformer.

### Applying a transformation

func applied(to: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Performs the composed transformation on a single input.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

TabularTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Sendable
- TabularTransformer
- Transformer

## See Also

### Composition

struct ComposedTransformer

A transformer that composes two transformers by applying them one after the other.

struct ComposedTemporalTransformer

A temporal transformer that composes two temporal transformers by applying them one after the other.

