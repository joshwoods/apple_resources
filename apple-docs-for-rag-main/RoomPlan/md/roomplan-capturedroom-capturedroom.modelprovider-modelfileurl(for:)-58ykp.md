

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
-  modelFileURL(for:) 

Instance Method

# modelFileURL(for:)

Provides a URL to the 3D model for the given attributes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func modelFileURL(for attributes: [any CapturedRoomAttribute]) throws -> URL?
```

## Parameters 

`attributes`  

An array of attributes that represent criteria for the model-URL query.

## Return Value

The 3D model that the app associates to the given object’s attributes via setModelFileURL(_:for:). If no 3D model URL associates to the given attribute combination, this function returns `nil`.

## Discussion

In error conditions, this function throws:

- CapturedRoom.ModelProvider.Error.nonExistingFile(url:) if a 3D model doesn’t exist at the given URL.

- CapturedRoom.ModelProvider.Error.attributeCombinationNotSupported if no object category supports all of the argument attributes.

Query supportedCombinations to check the attributes that an object category supports.

## See Also

### Managing models

var modelFileURLs: [URL]

An array of URLs to 3D models for all categories and attributes.

func modelFileURL(for: CapturedRoom.Object.Category) throws -> URL?

Provides a URL to the 3D model for the given category.

func modelFileURL(for: CapturedRoom.Object) throws -> URL?

Provides a URL to a 3D model based on the given object’s attributes or category.

func setModelFileURL(URL?, for: [any CapturedRoomAttribute]) throws

Associates a URL to the given attributes.

func setModelFileURL(URL?, for: CapturedRoom.Object.Category) throws

Associates a URL to the given object category.

