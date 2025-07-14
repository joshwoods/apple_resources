

- Automator
-  AMActionErrorKey 

Global Variable

# AMActionErrorKey

A key to retrieve the action that caused an error.

Mac Catalyst 14.0+macOS 10.4+

``` source
var AMActionErrorKey: String { get }
```

## Discussion

Use this key to obtain, from the userInfo dictionary of an instance of NSError, a reference to the action (AMAction) that caused the error.

## See Also

### Errors

var AMAutomatorErrorDomain: String

A string that identifies the Automator error domain.

struct AMError

An Automator error.

enum Code

Automator error codes.

