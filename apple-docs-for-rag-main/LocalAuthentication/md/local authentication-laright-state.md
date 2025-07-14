

- Local Authentication
- LARight
-  state 

Instance Property

# state

The current authorization state for a right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var state: LARight.State { get }
```

## See Also

### Monitoring authorization status

func checkCanAuthorize(completion: ((any Error)?) -> Void)

Checks whether the right has permission to perform authorization.

enum State

The possible states for a right during authorization.

