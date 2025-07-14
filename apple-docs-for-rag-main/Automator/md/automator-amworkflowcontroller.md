

- Automator
-  AMWorkflowController 

Class

# AMWorkflowController

An object that lets you manage an Automator workflow in your app.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMWorkflowController
```

## Overview

A controller can run and stop a workflow and obtain information about its state. The controller’s delegate (AMWorkflowControllerDelegate) receives messages as the workflow is executed and its actions are run.

You can load and run a workflow with minimal overhead by using the AMWorkflow class method run(at:withInput:). Use AMWorkflowController where you need greater control, such as the ability to start and stop the workflow. In that case, you must create and initialize both the workflow and the workflow controller objects.

## Topics

### Accessing the Workflow

var workflow: AMWorkflow?

The controller’s workflow.

### Accessing the Workflow View

var workflowView: AMWorkflowView?

The controller’s workflow view.

### Accessing the Delegate

var delegate: (any AMWorkflowControllerDelegate)?

The controller’s delegate.

protocol AMWorkflowControllerDelegate

A set of optional methods that a delegate of a workflow controller implements.

### Controlling the Workflow

func pause(Any)

Pauses a workflow that’s running.

func reset(Any)

Stops a workflow, clears any action results, and resets the workflow back to an un-run state.

func run(Any)

Runs the associated workflow, after first clearing any results stored by its actions during any previous run.

func step(Any)

In a paused workflow, runs the next action in the workflow and then pauses again.

func stop(Any)

Stops the associated workflow.

### Getting Workflow Information

var canRun: Bool

A Boolean value that indicates whether the controller’s workflow is able to run.

var isPaused: Bool

A Boolean value that indicates whether the controller’s workflow is currently paused.

var isRunning: Bool

A Boolean value that indicates whether the controller’s workflow is currently running.

## Relationships

### Inherits From

- NSController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSEditorRegistration
- NSObjectProtocol

## See Also

### Workflows

class AMWorkflow

An object that lets you use an Automator workflow in your app.

class AMWorkflowView

An object that lets you view and edit Automator workflows in your app.

class AMWorkspace

A workspace for running an Automator workflow.

