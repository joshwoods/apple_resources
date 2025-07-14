

- PHASE
- PHASEEnvelope
-  init(startPoint:segments:) 

Initializer

# init(startPoint:segments:)

Creates an envelope with a start point and segments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init?(
    startPoint: simd_double2,
    segments: [PHASEEnvelopeSegment]
)
```

## Parameters 

`startPoint`  

The start point of the envelope.

`segments`  

An array of segments.

## Discussion

For an empty `segments` argument, the resulting envelope contains one segment where the end point matches the start point. If the `segments` argument contains more than one segment, the resulting segments array sorts in ascending order on the *x* value.

Important

The start point’s *x* value must be less than or equal to the segment with the lowest *x* value of all other `segments`, otherwise this function returns `nil`.

