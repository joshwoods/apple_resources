

- SwiftUI
-  WKInterfaceObjectRepresentableContext 

Structure

# WKInterfaceObjectRepresentableContext

Contextual information about the state of the system that you use to create and update your WatchKit interface object.

watchOS 6.0+

``` source
@MainActor @preconcurrency
struct WKInterfaceObjectRepresentableContext where Representable : WKInterfaceObjectRepresentable
```

## Overview

A WKInterfaceObjectRepresentableContext structure contains details about the current state of the system. When creating and updating your interface objects, the system creates one of these structures and passes it to the appropriate method of your custom WKInterfaceObjectRepresentable instance. Use the information in this structure to configure your object. Don’t create this structure yourself.

## Topics

### Coordinating interactions

let coordinator: Representable.Coordinator

The view’s associated coordinator.

var transaction: Transaction

The current transaction.

### Getting the current environment data

var environment: EnvironmentValues

The current environment.

## Relationships

### Conforms To

- Sendable

## See Also

### Adding WatchKit views to SwiftUI view hierarchies

protocol WKInterfaceObjectRepresentable

A view that represents a WatchKit interface object.

