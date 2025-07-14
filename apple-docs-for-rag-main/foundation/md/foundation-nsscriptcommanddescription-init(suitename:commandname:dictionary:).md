

- Foundation
- NSScriptCommandDescription
-  init(suiteName:commandName:dictionary:) 

Initializer

# init(suiteName:commandName:dictionary:)

Initializes and returns a newly allocated instance of `NSScriptCommandDescription`.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(
    suiteName: String,
    commandName: String,
    dictionary commandDeclaration: [AnyHashable : Any]?
)
```

## Parameters 

`suiteName`  

The name of the suite (in the application’s scriptability information) that the command belongs to. For example, `"AppName Suite"`.

`commandName`  

The name of the script command that this instance describes.

`commandDeclaration`  

A command declaration dictionary of the sort that is valid in script suite property list files. This dictionary provides information about the command such as its argument names and types and return type (if any).

## Return Value

The initialized command description instance. Returns `nil` if the event constant or class name for the command description is missing; also returns `nil` if the return type or argument values are of the wrong type.

## Discussion

This method registers `self` with the application’s global instance of NSScriptSuiteRegistry and also registers all command arguments with the registry.

## See Also

### Related Documentation

Cocoa Scripting Guide

