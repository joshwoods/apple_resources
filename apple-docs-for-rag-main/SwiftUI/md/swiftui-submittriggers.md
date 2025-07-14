

- SwiftUI
-  SubmitTriggers 

Structure

# SubmitTriggers

A type that defines various triggers that result in the firing of a submission action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SubmitTriggers
```

## Overview

These triggers may be provided to the onSubmit(of:_:) modifier to alter which types of user behaviors trigger a provided submission action.

## Topics

### Getting submit triggers

static let search: SubmitTriggers

Defines triggers originating from search fields constructed from searchable modifiers.

static let text: SubmitTriggers

Defines triggers originating from text input controls like `TextField` and `SecureField`.

### Creating a set of options

init(rawValue: SubmitTriggers.RawValue)

Creates a set of submit triggers.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Responding to submission events

func onSubmit(of: SubmitTriggers, () -> Void) -> some View

Adds an action to perform when the user submits a value to this view.

func submitScope(Bool) -> some View

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

