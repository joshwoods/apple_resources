

- Automator
-  AMWorkflowView 

Class

# AMWorkflowView

An object that lets you view and edit Automator workflows in your app.

Mac Catalyst 14.0+macOS 10.4+

``` source
@MainActor
class AMWorkflowView
```

## Overview

A workflow view displays an instance of AMWorkflow.

You can use Interface Builder to add an instance of AMWorkflowView to a window in your app. You can then add an AMWorkflowView object to the nib window and use the controller’s workflowView outlet to connect it to the workflow view. The controller object also has run(_:) and stop(_:) actions that can be connected to buttons or other user interface elements.

## Topics

### Configuring the Workflow View

var isEditable: Bool

A Boolean value that indicates whether the workflow view is editable.

var workflowController: AMWorkflowController?

The view’s workflow controller.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Workflows

class AMWorkflow

An object that lets you use an Automator workflow in your app.

class AMWorkflowController

An object that lets you manage an Automator workflow in your app.

class AMWorkspace

A workspace for running an Automator workflow.

