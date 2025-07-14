

- Foundation
- NSScriptObjectSpecifier
-  evaluationError 

Instance Property

# evaluationError

Returns the object specifier in which an evaluation error occurred.

Mac Catalyst 13.0+macOS 10.0+

``` source
var evaluationError: NSScriptObjectSpecifier? { get }
```

## Return Value

The object specifier in which an evaluation error occurred.

## Discussion

The object specifier failing to evaluate could be the receiver or any container specifier “above” the receiver.

## See Also

### Getting evaluation errors

var evaluationErrorNumber: Int

Sets the value of the evaluation error.

