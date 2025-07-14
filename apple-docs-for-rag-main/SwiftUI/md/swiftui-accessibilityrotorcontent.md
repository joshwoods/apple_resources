

- SwiftUI
-  AccessibilityRotorContent 

Protocol

# AccessibilityRotorContent

Content within an accessibility rotor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
protocol AccessibilityRotorContent
```

## Overview

Generally generated from control flow constructs like `ForEach` and `if`, and `AccessibilityRotorEntry`.

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Supporting types

var body: Self.Body

The internal content of this `AccessibilityRotorContent`.

**Required**

associatedtype Body : AccessibilityRotorContent

The type for the internal content of this `AccessibilityRotorContent`.

**Required**

## Relationships

### Conforming Types

- AccessibilityRotorEntry

  Conforms when `ID` conforms to `Hashable`.

- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `AccessibilityRotorContent`.

- Group

  Conforms when `Content` conforms to `AccessibilityRotorContent`.

## See Also

### Creating rotors

struct AccessibilityRotorContentBuilder

Result builder you use to generate rotor entry content.

struct AccessibilityRotorEntry

A struct representing an entry in an Accessibility Rotor.

