

- Vision
- VNDetectHumanRectanglesRequest
-  upperBodyOnly 

Instance Property

# upperBodyOnly

A Boolean value that indicates whether the request requires detecting a full body or upper body only to produce a result.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var upperBodyOnly: Bool { get set }
```

## Discussion

The default value of true indicates that the request requires detecting a person’s upper body only to find the bound box around it.

