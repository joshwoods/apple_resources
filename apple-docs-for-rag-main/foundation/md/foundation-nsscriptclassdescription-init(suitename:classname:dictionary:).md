

- Foundation
- NSScriptClassDescription
-  init(suiteName:className:dictionary:) 

Initializer

# init(suiteName:className:dictionary:)

Initializes and returns a newly allocated instance of `NSScriptClassDescription`.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(
    suiteName: String,
    className: String,
    dictionary classDeclaration: [AnyHashable : Any]?
)
```

## Parameters 

`suiteName`  

The name of the suite (in the application’s scriptability information) that the class belongs to. For example, `"AppName Suite"`.

`className`  

The name of the class that this instance describes.

`classDeclaration`  

A class declaration dictionary of the sort that is valid in script suite property list files. This dictionary provides information about the class such as its attributes and relationships.

## Return Value

The initialized instance. Returns `nil` if the event code value for the class description itself is missing or is not an `NSString`. Also returns `nil` if the superclass name or any of the subdictionaries of descriptions are not of the right type.

## Discussion

This method registers `self` with the application’s global instance of NSScriptSuiteRegistry.

## See Also

### Related Documentation

Cocoa Scripting Guide

Key-Value Coding Programming Guide

