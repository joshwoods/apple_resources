

- SwiftUI
-  NSViewRepresentableContext 

Structure

# NSViewRepresentableContext

Contextual information about the state of the system that you use to create and update your AppKit view.

macOS 10.15+

``` source
@MainActor @preconcurrency
struct NSViewRepresentableContext where View : NSViewRepresentable
```

## Overview

An NSViewRepresentableContext structure contains details about the current state of the system. When creating and updating your view, the system creates one of these structures and passes it to the appropriate method of your custom NSViewRepresentable instance. Use the information in this structure to configure your view. For example, use the provided environment values to configure the appearance of your view. Don’t create this structure yourself.

## Topics

### Coordinating view-related interactions

let coordinator: View.Coordinator

An instance you use to communicate your AppKit view’s behavior and state out to SwiftUI objects.

var transaction: Transaction

The current transaction.

### Getting the current environment data

var environment: EnvironmentValues

Environment data that describes the current state of the system.

### Instance Methods

func animate(changes: () -> Void, completion: (() -> Void)?)

Animates changes using the animation in the current transaction.

## Relationships

### Conforms To

- Sendable

## See Also

### Adding AppKit views to SwiftUI view hierarchies

protocol NSViewRepresentable

A wrapper that you use to integrate an AppKit view into your SwiftUI view hierarchy.

protocol NSViewControllerRepresentable

A wrapper that you use to integrate an AppKit view controller into your SwiftUI interface.

struct NSViewControllerRepresentableContext

Contextual information about the state of the system that you use to create and update your AppKit view controller.

