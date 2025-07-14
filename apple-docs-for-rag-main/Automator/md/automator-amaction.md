

- Automator
-  AMAction 

Class

# AMAction

An abstract class that defines the interface and general characteristics of Automator actions.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMAction
```

## Overview

Automator is an Apple app that allows users to construct and execute workflows consisting of a sequence of discrete modules called actions. An action performs a specific task, such as copying a file or cropping an image, and passes its output to Automator to give to the next action in the workflow. Actions are currently implemented as loadable bundles owned by objects of the AMBundleAction class, a subclass of AMAction.

The critically important method declared by AMAction is run(withInput:). When Automator executes a workflow, it sends this message to each action object in the workflow (in workflow sequence), in most cases passing in the output of the previous action as input. The action object performs its task in this method and ends by returning an output object for the next action in the workflow.

Subclassing AMAction is not recommended. For most situations requiring an enhancement to the Automator framework, it is sufficient to subclass AMBundleAction.

## Topics

### Initializing and Encoding

init?(definition: [String : Any]?, fromArchive: Bool)

Initializes the action with the specified definition.

init(contentsOf: URL) throws

Loads an Automator action from a file URL.

func write(to: NSMutableDictionary)

Examines the parameters and other configuration information specified in the passed dictionary and adds its own information to it if appropriate.

### Controlling the Action

func run(withInput: Any?) throws -> Any

Requests the action to perform its task using the specified input.

func runAsynchronously(withInput: Any?)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

func finishRunningWithError((any Error)?)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

func willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

func stop()

Stops the action from running.

func reset()

Resets the action to its initial state.

### Initializing and Synchronizing the Action User Interface

func activated()

Allows the action to synchronize its information with settings in another app.

func opened()

Allows the action to initialize its user interface.

### Performing Logging

enum AMLogLevel

Logging levels that Automator supports.

### Updating Action Parameters

func parametersUpdated()

Requests the action to update its user interface from its stored parameters, which have changed.

func updateParameters()

Requests the action to update its stored set of parameters from the settings in the action’s user interface.

### Getting Action Information

var name: String

The name of the action.

var progressValue: CGFloat

A float value between 0 and 1, which indicates how far along the action is while processing.

var ignoresInput: Bool

A Boolean value that indicates whether the action acts upon its input or the input is ignored.

var output: Any?

The action’s output.

var selectedInputType: String?

The type of input, in UTI format, of the input received by the action.

var selectedOutputType: String?

The type of output, in UTI format, of the output to be produced by the action.

var isStopped: Bool

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

### Performing Cleanup Operations

func closed()

Invoked by Automator when the receiving action is removed from a workflow, allowing it to perform cleanup operations.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AMBundleAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Actions

class AMBundleAction

An object that represents an Automator action that’s a loadable bundle.

class AMShellScriptAction

An object that represents Automator actions whose runtime behavior is driven by a shell script or by a Perl or Python script.

