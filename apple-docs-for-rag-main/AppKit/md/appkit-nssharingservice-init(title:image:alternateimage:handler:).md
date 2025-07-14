

- AppKit
- NSSharingService
-  init(title:image:alternateImage:handler:) 

Initializer

# init(title:image:alternateImage:handler:)

Creates a custom sharing service object.

macOS 10.8+

``` source
init(
    title: String,
    image: NSImage,
    alternateImage: NSImage?,
    handler block: @escaping () -> Void
)
```

## Parameters 

`title`  

The custom sharing service name.

`image`  

The image that represents the sharing service

`alternateImage`  

The alternate image that represents the sharing service

`block`  

The block that actually interacts with the service.

## Return Value

An instance of the custom sharing object.

## Discussion

Custom sharing services can be added to the NSSharingServicePicker with the sharingServicePicker(_:sharingServicesForItems:proposedSharingServices:) delegate method.

When implementing this method, consider subclassing `NSSharingService` so the canPerform(withItems:) and sharingServices(forItems:) can provide accurate results.

## See Also

### Creating a Sharing Service

init?(named: NSSharingService.Name)

Returns a sharing service instance representing the specified service name.

struct Name

Constants that describe the sharing services that macOS supports.

