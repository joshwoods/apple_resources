

- Foundation
- NSScriptObjectSpecifier
-  init(descriptor:) 

Initializer

# init(descriptor:)

Returns a new object specifier for an Apple event descriptor.

macOS 10.5+

``` source
init?(descriptor: NSAppleEventDescriptor)
```

## Parameters 

`descriptor`  

An Apple event descriptor. The descriptor must have the type `typeObjectSpecifier`.

## Return Value

An object specifier, or `nil` if an error occurs.

## Discussion

If `objectSpecifierWithDescriptor:` is invoked and fails during the execution of a script command, information about the error that caused the failure is recorded in `[NSScriptCommand currentCommand]`.

## See Also

### Related Documentation

Cocoa Scripting Guide

