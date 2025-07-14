

- Playground Support
- PlaygroundPage
-  needsIndefiniteExecution 

Instance Property

# needsIndefiniteExecution

A Boolean value that indicates whether indefinite execution is enabled.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

**macOS**

``` source
final var needsIndefiniteExecution: Bool { get set }
```

**Swift Playgrounds**

``` source
var needsIndefiniteExecution: Bool { get set }
```

## Discussion

By default, all top-level code is executed, and then execution is terminated. When working with asynchronous code, enable indefinite execution to allow execution to continue after the end of the playground’s top-level code is reached. This, in turn, gives threads and callbacks time to execute.

With a traditional live view, editing the playground automatically stops execution, even when indefinite execution is enabled. When using the always-on live view, execution continues whether or not indefinite execution is enabled.

Set `needsIndefiniteExecution` to `true` to continue execution after the end of top-level code. Set it to `false` to stop execution at that point.

The default value is `false`. It's set to true when liveView is set to a non-`nil` value.

## See Also

### Configuring Execution

var executionMode: PlaygroundPage.ExecutionMode

The currently selected speed for executing the code on this playground page.

enum PlaygroundPage.ExecutionMode

The available speeds for executing the code on a playground page.

func finishExecution() -> Never

Terminates execution of the current playground page.

