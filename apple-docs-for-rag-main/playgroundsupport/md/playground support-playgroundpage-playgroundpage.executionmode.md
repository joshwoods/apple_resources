

- Playground Support
- PlaygroundPage
-  PlaygroundPage.ExecutionMode 

Enumeration

# PlaygroundPage.ExecutionMode

The available speeds for executing the code on a playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundPage.ExecutionMode
```

## Overview

The PlaygroundPage.ExecutionMode.run, PlaygroundPage.ExecutionMode.runFaster, and PlaygroundPage.ExecutionMode.runFastest modes all execute code immediately. The PlaygroundPage.ExecutionMode.step and PlaygroundPage.ExecutionMode.stepSlowly modes execute code statement by statement, highlighting each statement on the page as it's executed.

For faster execution, explicitly support the `PlaygroundPage.ExecutionMode.runFaster` and `PlaygroundPage.ExecutionMode.runFastest` modes in your live view code. These modes signal to you that the learner wants the live view to show progress faster than the normal speed. These execution options aren't displayed to the learner unless you opt in by adding the `MaximumSupportedExecutionSpeed` key to a page's manifest property list. Set the key to `Faster` or `Fastest`, depending on how many speeds your live view supports.

## Topics

### Controlling Execution Speed

case run

An execution mode that runs at the normal speed.

case runFaster

An execution mode that runs more quickly than usual.

case runFastest

An execution mode that runs at the fastest possible speed.

### Stepping Through Code

case step

An execution mode that executes code statement by statement.

case stepSlowly

An execution mode that executes code statement by statement with extra pauses between each.

### Comparing Modes

static func != (PlaygroundPage.ExecutionMode, PlaygroundPage.ExecutionMode) -> Bool

Returns `true` when the execution modes being compared are different.

## See Also

### Configuring Execution

var executionMode: PlaygroundPage.ExecutionMode

The currently selected speed for executing the code on this playground page.

var needsIndefiniteExecution: Bool

A Boolean value that indicates whether indefinite execution is enabled.

func finishExecution() -> Never

Terminates execution of the current playground page.

