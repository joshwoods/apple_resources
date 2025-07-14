

- Swift
-  ExpressibleByNilLiteral 

Protocol

# ExpressibleByNilLiteral

A type that can be initialized using the nil literal, `nil`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByNilLiteral : ~Copyable
```

## Overview

`nil` has a specific meaning in Swift—the absence of a value. Only the `Optional` type conforms to `ExpressibleByNilLiteral`. `ExpressibleByNilLiteral` conformance for types that use `nil` for other purposes is discouraged.

## Topics

### Initializers

init(nilLiteral: ())

Creates an instance initialized with `nil`.

**Required**

## Relationships

### Conforming Types

- Optional

  Conforms when `Wrapped` conforms to `Escapable`.

## See Also

### Value Literals

protocol ExpressibleByIntegerLiteral

A type that can be initialized with an integer literal.

protocol ExpressibleByFloatLiteral

A type that can be initialized with a floating-point literal.

protocol ExpressibleByBooleanLiteral

A type that can be initialized with the Boolean literals `true` and `false`.

struct StaticBigInt

An immutable arbitrary-precision signed integer.

