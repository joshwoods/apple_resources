

- Create ML Components
-  ComposedTemporalTransformer 

Structure

# ComposedTemporalTransformer

A temporal transformer that composes two temporal transformers by applying them one after the other.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ComposedTemporalTransformer where Inner : TemporalTransformer, Outer : TemporalTransformer, Inner.Output == Outer.Input
```

## Overview

The inner transformer’s output must match the outer transformer input. The result of this transformer is equivalent to invoking `outer(inner(x))` on an input `x`,

## Topics

### Creating the transformer

init(Inner, Outer)

Creates a transformer composition from two temporal transformers.

### Getting the properties

var inner: Inner

The inner transformer.

var outer: Outer

The outer transformer.

### Applying a transformer

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> ComposedTemporalTransformer&lt;Inner, Outer>.OutputSequence

Performs the composed transformation on an input sequence.

typealias Intermediate

The intermediate type.

typealias Input

The input type.

typealias Output

The output type.

typealias OutputSequence

The output sequence type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

TemporalTransformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Sendable
- TemporalTransformer

## See Also

### Composition

struct ComposedTransformer

A transformer that composes two transformers by applying them one after the other.

struct ComposedTabularTransformer

A transformer that composes two tabular transformers by applying them one after the other.

