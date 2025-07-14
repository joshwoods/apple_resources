

- Foundation
- Bundle
-  classNamed(\_:) 

Instance Method

# classNamed(\_:)

Returns the `Class` object for the specified name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func classNamed(_ className: String) -> AnyClass?
```

## Parameters 

`className`  

The name of a class.

## Return Value

The `Class` object for `className`. Returns `nil` if `className` is not one of the classes associated with the receiver or if there is an error loading the executable code containing the class implementation.

## Discussion

If the bundle’s executable code is not yet loaded, this method dynamically loads it into memory. Classes (and categories) are loaded from just one file within the bundle directory; this code file has the same name as the directory, but without the extension (”`.bundle`”, “`.app`”, “`.framework`”). As a side effect of code loading, the receiver posts didLoadNotification after all classes and categories have been loaded; see `Notifications` for details.

## See Also

### Related Documentation

func load() -> Bool

Dynamically loads the bundle’s executable code into a running program, if the code has not already been loaded.

### Getting Classes from a Bundle

var principalClass: AnyClass?

The bundle’s principal class.

class let didLoadNotification: NSNotification.Name

A notification that lets observers know when classes are dynamically loaded.

let NSLoadedClasses: String

A constant used as a key for the `userInfo` dictionary of a didLoadNotification notification that corresponds to an array of names of each class that was loaded.

