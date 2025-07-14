

- AVFoundation
-  AVAsyncProperty 

Class

# AVAsyncProperty

An asynchronous property that constrains its type and value.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AVAsyncProperty
```

## Mentioned in 

Loading media data asynchronously

## Overview

This class subclasses AVPartialAsyncProperty to provide a type constraint on the property value.

## Topics

### Accessing the Status

enum Status

Loaded status values for asynchronous properties.

## Relationships

### Inherits From

- AVPartialAsyncProperty

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Property loading

protocol AVAsynchronousKeyValueLoading

A protocol that defines the interface to load media data asynchronously.

class AVPartialAsyncProperty

An asynchronous property that constrains its type.

class AVAnyAsyncProperty

A base class for asynchronous properties.

