

- Vision
- VNDetectFaceLandmarksRequest
-  revision(\_:supportsConstellation:) 

Type Method

# revision(\_:supportsConstellation:)

Returns a Boolean value that indicates whether a revision supports a constellation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class func revision(
    _ requestRevision: Int,
    supportsConstellation constellation: VNRequestFaceLandmarksConstellation
) -> Bool
```

## Parameters 

`requestRevision`  

The revision of the request.

`constellation`  

The contellation for which to determine support.

## Return Value

true if the revision supports the constellation, otherwise false.

## See Also

### Identifying Request Revisions

let VNDetectFaceLandmarksRequestRevision3: Int

A constant for specifying revision 3 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision2: Int

A constant for specifying revision 2 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision1: Int

A constant for specifying revision 1 of the face landmarks detection request.

Deprecated

