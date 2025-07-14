

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
-  setModelFileURL(\_:for:) 

Instance Method

# setModelFileURL(\_:for:)

Associates a URL to the given attributes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
mutating func setModelFileURL(
    _ url: URL?,
    for attributes: [any CapturedRoomAttribute]
) throws
```

## Parameters 

`url`  

A URL to a 3D model.

`attributes`  

An array of attributes that represents a unique combination to which to associate the URL.

## Discussion

In error conditions, this function throws:

- CapturedRoom.ModelProvider.Error.nonExistingFile(url:) if a 3D model doesn’t exist at the given URL.

- CapturedRoom.ModelProvider.Error.attributeCombinationNotSupported if no object category supports all of the argument attributes.

Query supportedCombinations to check the attributes that a category supports.

## See Also

### Managing models

var modelFileURLs: [URL]

An array of URLs to 3D models for all categories and attributes.

func modelFileURL(for: CapturedRoom.Object.Category) throws -> URL?

Provides a URL to the 3D model for the given category.

func modelFileURL(for: CapturedRoom.Object) throws -> URL?

Provides a URL to a 3D model based on the given object’s attributes or category.

func modelFileURL(for: [any CapturedRoomAttribute]) throws -> URL?

Provides a URL to the 3D model for the given attributes.

func setModelFileURL(URL?, for: CapturedRoom.Object.Category) throws

Associates a URL to the given object category.

