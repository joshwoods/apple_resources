

- Foundation
- NSCreateCommand
-  createClassDescription 

Instance Property

# createClassDescription

Returns the class description for the class that is to be created.

Mac Catalyst 13.0+macOS 10.0+

``` source
var createClassDescription: NSScriptClassDescription { get }
```

## Return Value

The class description for the class that is to be created.

## See Also

### Related Documentation

Cocoa Scripting Guide

### Getting information about a create command

var resolvedKeyDictionary: [String : Any]

Returns a dictionary that contains the properties that were specified in the `make` Apple event command that has been converted to this `NSCreateCommand` object.

