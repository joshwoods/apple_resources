

- Foundation
-  NSLoadedClasses 

Global Variable

# NSLoadedClasses

A constant used as a key for the `userInfo` dictionary of a didLoadNotification notification that corresponds to an array of names of each class that was loaded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSLoadedClasses: String
```

## See Also

### Getting Classes from a Bundle

func classNamed(String) -> AnyClass?

Returns the `Class` object for the specified name.

var principalClass: AnyClass?

The bundle’s principal class.

class let didLoadNotification: NSNotification.Name

A notification that lets observers know when classes are dynamically loaded.

