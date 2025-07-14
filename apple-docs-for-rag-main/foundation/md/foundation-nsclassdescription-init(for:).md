

- Foundation
- NSClassDescription
-  init(for:) 

Initializer

# init(for:)

Returns the class description for a given class.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(for aClass: AnyClass)
```

## Parameters 

`aClass`  

The class for which to return a class description. See note below for important details.

## Return Value

The class description for `aClass`, or `nil` if a class description cannot be found.

## Discussion

If a class description for `aClass` is not found, the method posts an NSClassDescriptionNeededForClassNotification on behalf of `aClass`, allowing an observer to register a class description. The method then checks for a class description again. Returns `nil` if a class description is still not found.

If you have an instance of the receiver’s class, you can use the `NSObject` instance method classDescription instead.

Note

In macOS 10.6 and later, this method (and as a result classDescription methods of any object) will return `nil` when the sdef contains no `` element for the Cocoa class, but there is a `` element defined for a superclass.

This is incorrect, as object instances should never be required to be exactly a given class, any class should be allowed to be a subclass of the required class and receive the correct `` value.

This situation can have a serious impact on Cocoa Scripting, and there is no plan on changing this behavior.

Instead of using this method, you should use the init(for:) method of NSScriptClassDescription instead.

## See Also

### Related Documentation

Cocoa Scripting Guide

Key-Value Coding Programming Guide

### Working with class descriptions

class func invalidateClassDescriptionCache()

Removes all `NSClassDescription` objects from the cache.

class func register(NSClassDescription, for: AnyClass)

Registers an `NSClassDescription` object for a given class in the `NSClassDescription` cache.

