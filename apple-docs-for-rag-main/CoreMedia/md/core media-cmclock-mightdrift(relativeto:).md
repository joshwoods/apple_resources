

- Core Media
- CMClock
-  mightDrift(relativeTo:) 

Instance Method

# mightDrift(relativeTo:)

Returns a Boolean value that indicates whether it’s possible for one timebase or clock to drift relative to another.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func mightDrift(relativeTo otherClock: CMClock) -> Bool
```

## Parameters 

`otherClock`  

The clock to compare to.

