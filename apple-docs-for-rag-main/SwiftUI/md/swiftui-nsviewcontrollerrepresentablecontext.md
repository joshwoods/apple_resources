

- SwiftUI
-  NSViewControllerRepresentableContext 

Structure

# NSViewControllerRepresentableContext

Contextual information about the state of the system that you use to create and update your AppKit view controller.

macOS 10.15+

``` source
@MainActor @preconcurrency
struct NSViewControllerRepresentableContext where ViewController : NSViewControllerRepresentable
```

## Overview

An NSViewControllerRepresentableContext structure contains details about the current state of the system. When creating and updating your view controller, the system creates one of these structures and passes it to the appropriate method of your custom NSViewControllerRepresentable instance. Use the information in this structure to configure your view controller. For example, use the provided environment values to configure the appearance of your view controller and views. Don’t create this structure yourself.

## Topics

### Coordinating view-related interactions

let coordinator: ViewController.Coordinator

An object you use to communicate your AppKit view controller’s behavior and state out to SwiftUI objects.

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

struct NSViewRepresentableContext

Contextual information about the state of the system that you use to create and update your AppKit view.

protocol NSViewControllerRepresentable

A wrapper that you use to integrate an AppKit view controller into your SwiftUI interface.

