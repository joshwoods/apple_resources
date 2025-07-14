

- Image Playground
- ImageCreator
-  init() 

Initializer

# init()

Creates a new image creator object for you to use in your app.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
init() async throws
```

## Discussion

If the device doesn’t support image creation or the feature is currently unavailable, this initializer throws an error.

