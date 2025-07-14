

- Automator
-  AMWorkflow 

Class

# AMWorkflow

An object that lets you use an Automator workflow in your app.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMWorkflow
```

## Overview

A *workflow* consists of one or more actions, discrete tasks which together can perform complex automation tasks. Your app can use workflows to package its own features and to take advantage of features provided by other apps. You create actions with Xcode, while you create workflows with the Automator app.

You can load and run a workflow with minimal overhead by using the class method run(at:withInput:). However, in situations where you need greater control, such as the ability to start and stop the workflow, you can use an instance of the AMWorkflowController class instead. In that case, you must create and initialize both the workflow and the workflow controller objects.

In either case, the workflow runs in a separate process so that any actions it contains are executed in a separate memory space. That helps to insulate your app from crashes, memory leaks, or exceptions that might occur from running the actions in the workflow.

You can display a workflow with an instance of AMWorkflowView.

## Topics

### Creating a Workflow

init()

Creates and initializes a workflow.

convenience init(contentsOf: URL) throws

Creates and initializes a workflow based on the contents of the specified file.

### Running a Workflow

class func run(at: URL, withInput: Any?) throws -> Any

Loads and runs the specified workflow file.

### Saving Changes to a Workflow

func write(to: URL) throws

Writes the workflow to the specified file.

### Getting Information About a Workflow

var actions: [AMAction]

An array of the workflow’s actions.

var fileURL: URL?

A URL that specifies the location of the workflow file.

func valueForVariable(withName: String) -> Any?

Returns the value of the workflow variable with the specified name.

### Working with the Workflow’s Input and Output

var input: Any?

The input data that is passed to the first action in the workflow.

var output: Any?

The output data that is provided by the last action in the workflow.

### Manipulating the Workflow

func setValue(Any?, forVariableWithName: String) -> Bool

Sets the value of the workflow variable with the specified name.

### Manipulating the Workflow’s Actions

func addAction(AMAction)

Adds the specified action at the end of the receiving workflow.

func insertAction(AMAction, at: Int)

Inserts the specified action at the specified position of the receiving workflow.

func moveAction(at: Int, to: Int)

Moves the action from the specified start position to the specified end position in the receiving workflow.

func removeAction(AMAction)

Removes the specified action from the workflow.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Workflows

class AMWorkflowController

An object that lets you manage an Automator workflow in your app.

class AMWorkflowView

An object that lets you view and edit Automator workflows in your app.

class AMWorkspace

A workspace for running an Automator workflow.

