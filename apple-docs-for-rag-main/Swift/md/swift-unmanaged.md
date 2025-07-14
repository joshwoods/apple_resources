

- Swift
-  Unmanaged 

Structure

# Unmanaged

A type for propagating an unmanaged object reference.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Unmanaged where Instance : AnyObject
```

## Mentioned in 

Working with Core Foundation Types

## Overview

When you use this type, you become partially responsible for keeping the object alive.

## Topics

### Instance Methods

func autorelease() -> Unmanaged&lt;Instance>

Performs an unbalanced autorelease of the object.

func release()

Performs an unbalanced release of the object.

func retain() -> Unmanaged&lt;Instance>

Performs an unbalanced retain of the object.

func takeRetainedValue() -> Instance

Gets the value of this unmanaged reference as a managed reference and consumes an unbalanced retain of it.

func takeUnretainedValue() -> Instance

Gets the value of this unmanaged reference as a managed reference without consuming an unbalanced retain of it.

func toOpaque() -> UnsafeMutableRawPointer

Unsafely converts an unmanaged class reference to a pointer.

### Type Methods

static func fromOpaque(UnsafeRawPointer) -> Unmanaged&lt;Instance>

Unsafely turns an opaque C pointer into an unmanaged class reference.

static func passRetained(Instance) -> Unmanaged&lt;Instance>

Creates an unmanaged reference with an unbalanced retain.

static func passUnretained(Instance) -> Unmanaged&lt;Instance>

Creates an unmanaged reference without performing an unbalanced retain.

### Default Implementations

AtomicOptionalRepresentable Implementations

AtomicRepresentable Implementations

## Relationships

### Conforms To

- AtomicOptionalRepresentable

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- AtomicRepresentable

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- BitwiseCopyable

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- Copyable

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- Sendable

  Conforms when `Instance` conforms to `Copyable`, `Escapable`, and `Sendable`.

## See Also

### Reference Counting

func withExtendedLifetime&lt;T, E, Result>(borrowing T, (borrowing T) throws(E) -> Result) throws(E) -> Result

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

func withExtendedLifetime&lt;T, E, Result>(borrowing T, () throws(E) -> Result) throws(E) -> Result

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

