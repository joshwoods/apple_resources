

- Foundation
- Bundle
-  didLoadNotification 

Type Property

# didLoadNotification

A notification that lets observers know when classes are dynamically loaded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let didLoadNotification: NSNotification.Name
```

## Discussion

When a request is made to a bundle for a class (classNamed(_:) or principalClass), the bundle dynamically loads the executable code file that contains the class implementation and all other class definitions contained in the file. After the module is loaded, the bundle posts the didLoadNotification.

The notification object is the Bundle instance that dynamically loads classes. The `userInfo` dictionary contains an NSLoadedClasses key.

In a typical use of this notification, an object might want to enumerate the `userInfo` array to check if each loaded class conformed to a certain protocol (say, an protocol for a plug-and-play tool set); if a class does conform, the object would create an instance of that class and add the instance to another NSArray object.

## See Also

### Getting Classes from a Bundle

func classNamed(String) -> AnyClass?

Returns the `Class` object for the specified name.

var principalClass: AnyClass?

The bundle’s principal class.

let NSLoadedClasses: String

A constant used as a key for the `userInfo` dictionary of a didLoadNotification notification that corresponds to an array of names of each class that was loaded.

