

- AVFoundation
- AVMediaDataStorage
-  init(url:options:) 

Initializer

# init(url:options:)

Creates a media data storage object associated with a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
init(
    url URL: URL,
    options: [String : Any]? = nil
)
```

## Parameters 

`URL`  

The URL specifying where sample data added to a movie or track is written.

`options`  

A dictionary object containing keys for specifying initialization options. No keys are currently defined.

## Return Value

An `AVMediaDataStorage` object.

