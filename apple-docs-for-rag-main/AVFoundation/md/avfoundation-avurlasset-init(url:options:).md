

- AVFoundation
- AVURLAsset
-  init(url:options:) 

Initializer

# init(url:options:)

Creates an asset that models the media resource at the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    url URL: URL,
    options: [String : Any]? = nil
)
```

## Parameters 

`URL`  

A URL that references the media for the asset to model.

`options`  

A dictionary that contains options used to customize the initialization of the asset.

For supported keys and values, see Initialization Options.

## Return Value

An asset that models the media resource found at `URL`.

## See Also

### Creating an Asset

convenience init(url: URL)

Creates an asset that models the media at the specified URL.

Initialization Options

Specify options to configure the initialization of a media asset.

