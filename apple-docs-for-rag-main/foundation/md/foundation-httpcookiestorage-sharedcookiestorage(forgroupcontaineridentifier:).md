

- Foundation
- HTTPCookieStorage
-  sharedCookieStorage(forGroupContainerIdentifier:) 

Type Method

# sharedCookieStorage(forGroupContainerIdentifier:)

Returns the cookie storage instance for the container associated with the specified app group identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func sharedCookieStorage(forGroupContainerIdentifier identifier: String) -> HTTPCookieStorage
```

## Parameters 

`identifier`  

The app group identifier.

## Discussion

By default, apps and associated app extensions will have different data containers. As a result, the value of the HTTPCookieStorage class’s shared property will refer to different persistent cookie stores when called by the app and by its extensions.You can use this method to create a persistent cookie storage available to all apps and extensions with access to the same app group.

Subsequent calls to the this method with the same identifier will return the same storage instance.

## See Also

### Getting the shared cookie storage object

class var shared: HTTPCookieStorage

The shared cookie storage instance.

