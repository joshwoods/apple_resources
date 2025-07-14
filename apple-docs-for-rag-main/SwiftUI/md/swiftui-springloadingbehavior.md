

- SwiftUI
-  SpringLoadingBehavior 

Structure

# SpringLoadingBehavior

The options for controlling the spring loading behavior of views.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SpringLoadingBehavior
```

## Overview

Use values of this type with the springLoadingBehavior(_:) modifier.

## Topics

### Getting the behaviors

static let automatic: SpringLoadingBehavior

The automatic spring loading behavior.

static let enabled: SpringLoadingBehavior

Spring loaded interactions will be enabled for applicable views.

static let disabled: SpringLoadingBehavior

Spring loaded interactions will be disabled for applicable views.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring spring loading

func springLoadingBehavior(SpringLoadingBehavior) -> some View

Sets the spring loading behavior this view.

var springLoadingBehavior: SpringLoadingBehavior

The behavior of spring loaded interactions for the views associated with this environment.

