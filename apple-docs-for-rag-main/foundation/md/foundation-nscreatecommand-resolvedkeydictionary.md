

- Foundation
- NSCreateCommand
-  resolvedKeyDictionary 

Instance Property

# resolvedKeyDictionary

Returns a dictionary that contains the properties that were specified in the `make` Apple event command that has been converted to this `NSCreateCommand` object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var resolvedKeyDictionary: [String : Any] { get }
```

## Return Value

A dictionary that contains the properties that were specified in the `make` Apple event script command that has been converted to this `NSCreateCommand` object.

## Discussion

The keys in the returned dictionary are the names of properties (attributes or relationships, in the script suite) that have been specified for the command, and the corresponding values in the dictionary are the values that those properties should take. The required and optional arguments for the `make` command are specified in the core suite definition, `NSCoreSuite.scriptSuite`.

## See Also

### Getting information about a create command

var createClassDescription: NSScriptClassDescription

Returns the class description for the class that is to be created.

