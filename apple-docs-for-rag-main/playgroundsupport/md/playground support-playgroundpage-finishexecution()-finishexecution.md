

- Playground Support
- PlaygroundPage
-  finishExecution() 

Instance Method

# finishExecution()

Terminates execution of the current playground page.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

**macOS**

``` source
final func finishExecution() -> Never
```

**Swift Playgrounds**

``` source
func finishExecution() -> Never
```

## Discussion

This function immediately terminates any code running in the playground. Call this function when you've set `needsIndefiniteExecution` to `true` to indicate that the indefinite period of code execution has ended.

## See Also

### Configuring Execution

var executionMode: PlaygroundPage.ExecutionMode

The currently selected speed for executing the code on this playground page.

enum PlaygroundPage.ExecutionMode

The available speeds for executing the code on a playground page.

var needsIndefiniteExecution: Bool

A Boolean value that indicates whether indefinite execution is enabled.

