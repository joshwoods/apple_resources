

- Foundation
- NSScriptCommand
-  arguments 

Instance Property

# arguments

Sets the arguments of the command to `args`.

Mac Catalyst 13.0+macOS 10.0+

``` source
var arguments: [String : Any]? { get set }
```

## Discussion

Each argument in the dictionary is identified by the same name key used for the argument in the command’s class declaration in the script suite file.

## See Also

### Accessing arguments

var evaluatedArguments: [String : Any]?

Returns a dictionary containing the arguments of the command, evaluated from object specifiers to objects if necessary. The keys in the dictionary are the argument names.

