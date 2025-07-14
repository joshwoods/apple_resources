

- Core Data
- NSPersistentContainer
-  defaultDirectoryURL() 

Type Method

# defaultDirectoryURL()

Returns the location of the directory that contains the persistent stores.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func defaultDirectoryURL() -> URL
```

## Return Value

An NSURL that references the directory in which the persistent store(s) will be located or are currently located.

## Discussion

This method returns a platform-dependent NSURL at which the persistent store(s) will be located or are currently located. This method can be overridden in a subclass of NSPersistentContainer.

## See Also

### Accessing the Default Directory

class var defaultDirectoryURL: URL

The location of the directory that contains the persistent stores.

