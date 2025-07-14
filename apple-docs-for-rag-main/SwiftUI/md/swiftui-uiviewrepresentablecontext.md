

- SwiftUI
-  UIViewRepresentableContext 

Structure

# UIViewRepresentableContext

Contextual information about the state of the system that you use to create and update your UIKit view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct UIViewRepresentableContext where Representable : UIViewRepresentable
```

## Overview

A UIViewRepresentableContext structure contains details about the current state of the system. When creating and updating your view, the system creates one of these structures and passes it to the appropriate method of your custom UIViewRepresentable instance. Use the information in this structure to configure your view. For example, use the provided environment values to configure the appearance of your view. Don’t create this structure yourself.

## Topics

### Coordinating view-related interactions

let coordinator: Representable.Coordinator

The view’s associated coordinator.

var transaction: Transaction

The current transaction.

### Getting the current environment data

var environment: EnvironmentValues

The current environment.

### Instance Methods

func animate(changes: () -> Void, completion: (() -> Void)?)

Animates changes using the animation in the current transaction.

## Relationships

### Conforms To

- Sendable

## See Also

### Adding UIKit views to SwiftUI view hierarchies

protocol UIViewRepresentable

A wrapper for a UIKit view that you use to integrate that view into your SwiftUI view hierarchy.

protocol UIViewControllerRepresentable

A view that represents a UIKit view controller.

struct UIViewControllerRepresentableContext

Contextual information about the state of the system that you use to create and update your UIKit view controller.

