

- Swift Testing
-  Confirmation 

Structure

# Confirmation

A type that can be used to confirm that an event occurs zero or more times.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Confirmation
```

## Mentioned in 

Migrating a test from XCTest

Testing asynchronous code

## Topics

### Instance Methods

func callAsFunction(count: Int)

Confirm this confirmation.

func confirm(count: Int)

Confirm this confirmation.

## Relationships

### Conforms To

- Sendable

## See Also

### Confirming that asynchronous events occur

Testing asynchronous code

Validate whether your code causes expected events to happen.

func confirmation&lt;R>(Comment?, expectedCount: Int, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, (Confirmation) async throws -> sending R) async rethrows -> R

Confirm that some event occurs during the invocation of a function.

func confirmation&lt;R>(Comment?, expectedCount: some RangeExpression&lt;Int> &amp; Sendable &amp; Sequence&lt;Int>, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, (Confirmation) async throws -> sending R) async rethrows -> R

Confirm that some event occurs during the invocation of a function.

