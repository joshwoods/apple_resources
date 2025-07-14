

- Playground Support
- PlaygroundPage
-  executionMode 

Instance Property

# executionMode

The currently selected speed for executing the code on this playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
var executionMode: PlaygroundPage.ExecutionMode { get set }
```

## See Also

### Configuring Execution

enum PlaygroundPage.ExecutionMode

The available speeds for executing the code on a playground page.

var needsIndefiniteExecution: Bool

A Boolean value that indicates whether indefinite execution is enabled.

func finishExecution() -> Never

Terminates execution of the current playground page.

