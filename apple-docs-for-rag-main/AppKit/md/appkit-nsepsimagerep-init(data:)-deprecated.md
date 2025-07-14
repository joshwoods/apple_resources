

- AppKit
- NSEPSImageRep
-  init(data:) Deprecated

Initializer

# init(data:)

Returns a representation of an image initialized with the specified EPS data.

macOS 10.0–14.0Deprecated

``` source
init?(data epsData: Data)
```

Deprecated

\`NSEPSImageRep\` instances cannot be created on macOS 14.0 and later

## Parameters 

`epsData`  

The EPS data representing the desired image.

## Return Value

The initialized `NSEPSImageRep` object or `nil` if the object could not be initialized

## Discussion

The size of the receiver is set using the bounding box information specified in the EPS header comments.

