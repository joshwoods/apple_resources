

- Foundation
- NSScriptObjectSpecifier
-  objectsByEvaluatingSpecifier 

Instance Property

# objectsByEvaluatingSpecifier

Returns the actual object represented by the nested series of object specifiers.

Mac Catalyst 13.0+macOS 10.0+

``` source
var objectsByEvaluatingSpecifier: Any? { get }
```

## Return Value

The actual object represented by the nested series of object specifiers.

## Discussion

Recursively obtains the next container in a nested series of object specifiers until it reaches the top-level container specifier (which is either an NSWhoseSpecifier or the application object), after which it begins evaluating each object specifier (objectsByEvaluating(withContainers:)) going in the opposite direction (top-level to innermost) as it unwinds from the stack. Returns the actual object represented by the nested series of object specifiers. Returns `nil` if a container specifier could not be evaluated or if no top-level container specifier could be found. Thus `nil` can be a valid value or can indicate an error; you can use evaluationErrorNumber to determine if and which error occurred and evaluationError to find the container specifier responsible for the error. In the normal course of command processing, this method is invoked by an `NSScriptCommand` object’s evaluatedArguments and evaluatedReceivers methods, which take as message receiver the innermost object specifier.

## See Also

### Evaluating an object specifier

func indicesOfObjectsByEvaluating(withContainer: Any, count: UnsafeMutablePointer&lt;Int>) -> UnsafeMutablePointer&lt;Int>?

This primitive method must be overridden by subclasses to return a pointer to an array of indices identifying objects in the key of a given container that are identified by the receiver of the message.

func objectsByEvaluating(withContainers: Any) -> Any?

Returns the actual object or objects specified by the receiver as evaluated in the context of given container object.

