

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
-  modelFileURLs 

Instance Property

# modelFileURLs

An array of URLs to 3D models for all categories and attributes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var modelFileURLs: [URL] { get }
```

## See Also

### Managing models

func modelFileURL(for: CapturedRoom.Object.Category) throws -> URL?

Provides a URL to the 3D model for the given category.

func modelFileURL(for: CapturedRoom.Object) throws -> URL?

Provides a URL to a 3D model based on the given object’s attributes or category.

func modelFileURL(for: [any CapturedRoomAttribute]) throws -> URL?

Provides a URL to the 3D model for the given attributes.

func setModelFileURL(URL?, for: [any CapturedRoomAttribute]) throws

Associates a URL to the given attributes.

func setModelFileURL(URL?, for: CapturedRoom.Object.Category) throws

Associates a URL to the given object category.

