

- GameKit
- GKMatchmaker
-  shared() 

Type Method

# shared()

Returns the singleton matchmaker instance.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class func shared() -> GKMatchmaker
```

## Return Value

The shared matchmaker instance.

## Discussion

Games don’t create a `GKMatchmaker` object. Use this method instead to get the shared singleton instance.

