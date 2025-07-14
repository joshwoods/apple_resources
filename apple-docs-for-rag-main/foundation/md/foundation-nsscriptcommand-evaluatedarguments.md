

- Foundation
- NSScriptCommand
-  evaluatedArguments 

Instance Property

# evaluatedArguments

Returns a dictionary containing the arguments of the command, evaluated from object specifiers to objects if necessary. The keys in the dictionary are the argument names.

Mac Catalyst 13.0+macOS 10.0+

``` source
var evaluatedArguments: [String : Any]? { get }
```

## Discussion

Arguments initially can be either a normal object or an object specifier such as `word 5` (represented as an instance of an `NSScriptObjectSpecifier` subclass). If arguments are object specifiers, the receiver evaluates them before using the referenced objects. Returns `nil` if the command is not well formed. Also returns `nil` if an object specifier does not evaluate to an object or if there is no type defined for the argument in the command description.

## See Also

### Related Documentation

var isWellFormed: Bool

Returns a Boolean value indicating whether the receiver is well formed according to its command description.

### Accessing arguments

var arguments: [String : Any]?

Sets the arguments of the command to `args`.

