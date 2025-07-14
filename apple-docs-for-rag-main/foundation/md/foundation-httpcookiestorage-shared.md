

- Foundation
- HTTPCookieStorage
-  shared 

Type Property

# shared

The shared cookie storage instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var shared: HTTPCookieStorage { get }
```

## See Also

### Getting the shared cookie storage object

class func sharedCookieStorage(forGroupContainerIdentifier: String) -> HTTPCookieStorage

Returns the cookie storage instance for the container associated with the specified app group identifier.

