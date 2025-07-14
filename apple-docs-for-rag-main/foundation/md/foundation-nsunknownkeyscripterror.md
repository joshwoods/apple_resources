

- Foundation
-  NSUnknownKeyScriptError 

Global Variable

# NSUnknownKeyScriptError

An unidentified error occurred; indicates an error in the scripting support of your application.

Mac Catalyst 13.0+macOS 10.0+

``` source
var NSUnknownKeyScriptError: Int { get }
```

## See Also

### Constants

var NSNoScriptError: Int

No error.

var NSReceiverEvaluationScriptError: Int

The object or objects specified by the direct parameter to a command could not be found.

var NSKeySpecifierEvaluationScriptError: Int

The object or objects specified by a key (for commands that support key specifiers) could not be found.

var NSArgumentEvaluationScriptError: Int

The object specified by an argument could not be found.

var NSReceiversCantHandleCommandScriptError: Int

The receivers don’t support the command sent to them.

var NSRequiredArgumentsMissingScriptError: Int

An argument (or more than one argument) is missing.

var NSArgumentsWrongScriptError: Int

An argument (or more than one argument) is of the wrong type or is otherwise invalid.

var NSInternalScriptError: Int

An unidentified internal error occurred; indicates an error in the scripting support of your application.

var NSOperationNotSupportedForKeyScriptError: Int

The implementation of a scripting command signaled an error.

var NSCannotCreateScriptCommandError: Int

Could not create the script command; an invalid or unrecognized Apple event was received.

