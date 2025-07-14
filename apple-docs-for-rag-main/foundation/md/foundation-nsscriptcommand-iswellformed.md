

- Foundation
- NSScriptCommand
-  isWellFormed 

Instance Property

# isWellFormed

Returns a Boolean value indicating whether the receiver is well formed according to its command description.

Mac Catalyst 13.0+macOS 10.0+

``` source
var isWellFormed: Bool { get }
```

## Discussion

The method ensures that there is a description of the command and that the number of arguments and the types of non-specifier arguments conform to the command description.

## See Also

### Getting command information

var commandDescription: NSScriptCommandDescription

Returns the command description for the command.

