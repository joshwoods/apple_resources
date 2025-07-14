

- AppKit
- NSSharingService
-  init(named:) 

Initializer

# init(named:)

Returns a sharing service instance representing the specified service name.

macOS 10.8+

``` source
init?(named serviceName: NSSharingService.Name)
```

## Parameters 

`serviceName`  

The service name. The possible system provided values are listed in `Available Sharing Services`.

## Return Value

An instance of `NSSharingService` for the specified service name.

## See Also

### Related Documentation

class func sharingServices(forItems: [Any]) -> [NSSharingService]

Returns a list of sharing services which could share all the provided items together.

Deprecated

func canPerform(withItems: [Any]?) -> Bool

Returns whether the service can share all the specified items.

### Creating a Sharing Service

init(title: String, image: NSImage, alternateImage: NSImage?, handler: () -> Void)

Creates a custom sharing service object.

struct Name

Constants that describe the sharing services that macOS supports.

