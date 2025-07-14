

- StoreKit
- ProductIconPhase
-  ProductIconPhase.failure(\_:) 

Case

# ProductIconPhase.failure(\_:)

The promotional image failed to load, with an error.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case failure(any Error)
```

## Parameters 

`Error`  

The reason that the promotional image failed to load.

## See Also

### Getting the promotional image’s load phases

case loading

The promotional image is in the process of loading.

case success(Image)

The promotional image successfully loaded.

case unavailable

The promotional image isn’t available for download.

