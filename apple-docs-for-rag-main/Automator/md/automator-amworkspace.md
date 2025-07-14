

- Automator
-  AMWorkspace 

Class

# AMWorkspace

A workspace for running an Automator workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMWorkspace
```

## Overview

The AMWorkspace class provides access to the shared workspace in the Automator framework, where you can run workflows without a workflow controller. Use shared to access the shared workspace and runWorkflow(atPath:withInput:) to run your workflow in it.

## Topics

### Accessing the Shared Workspace

class var shared: AMWorkspace!

The shared workspace object.

### Running Workflows

func runWorkflow(atPath: String!, withInput: Any!) throws -> Any

Loads and runs the specified workflow file.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Workflows

class AMWorkflow

An object that lets you use an Automator workflow in your app.

class AMWorkflowController

An object that lets you manage an Automator workflow in your app.

class AMWorkflowView

An object that lets you view and edit Automator workflows in your app.

