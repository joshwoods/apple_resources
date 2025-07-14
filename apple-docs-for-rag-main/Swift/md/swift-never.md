

- Swift
-  Never 

Enumeration

# Never

A type that has no values and can’t be constructed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum Never
```

## Overview

Use `Never` as the return type of a function that doesn’t return normally — for example, because it runs forever or terminates the program.

```
// An infinite loop never returns.
func forever() -> Never {
    while true {
        print("I will print forever.")
    }
}

// Calling fatalError(_:file:line:) unconditionally stops the program.
func crashAndBurn() -> Never {
    fatalError("Something very, very bad happened")
}
```

A function that returns `Never` is called a *nonreturning* function. Closures, methods, computed properties, and subscripts can also be nonreturning.

There’s no way to create an instance of `Never`; this characteristic makes it an *uninhabited* type. You can use an uninhabited type like `Never` to represent states in your program that are impossible to reach during execution. Swift’s type system uses this information — for example, to reason about control statements in cases that are known to be unreachable.

```
let favoriteNumber: Result = .success(42)
switch favoriteNumber {
case .success(let value):
    print("My favorite number is", value)
}
```

In the code above, `favoriteNumber` has a failure type of `Never`, indicating that it always succeeds. The switch statement is therefore exhaustive, even though it doesn’t contain a `.failure` case, because that case could never be reached.

## Topics

### Type Aliases

typealias MapContentValue

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;Never>

### Default Implementations

AppIntent Implementations

AtomicRepresentable Implementations

AttachmentContent Implementations

Comparable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Identifiable Implementations

IntentResult Implementations

ParameterSummary Implementations

PersistentlyIdentifiable Implementations

TestScoping Implementations

TransferRepresentation Implementations

Transferable Implementations

## Relationships

### Conforms To

- AccessibilityRotorContent
- AppExtensionScene
- AppIntent
- AtomicRepresentable
- AttachmentContent
- AxisContent
- AxisMark
- BitwiseCopyable
- ChartContent
- Commands
- Comparable
- ControlWidgetConfiguration
- ControlWidgetTemplate
- Copyable
- CustomHoverEffect
- CustomizableToolbarContent
- Decodable
- Encodable
- Equatable
- Error
- Gesture
- Hashable
- Identifiable
- ImmersiveSpaceContent
- IntentResult
- Keyframes
- MapContent
- MapSelectable
- ParameterSummary
- PersistentlyIdentifiable
- Plottable
- PrimitivePlottableProtocol
- Scene
- Sendable
- ShapeStyle
- SortComparator
- StoreContent
- TableColumnContent
- TableRowContent
- TestScoping
- ToolbarContent
- TransferRepresentation
- Transferable
- View
- WidgetConfiguration

## See Also

### Exiting a Program

func fatalError(@autoclosure () -> String, file: StaticString, line: UInt) -> Never

Unconditionally prints a given message and stops execution.

