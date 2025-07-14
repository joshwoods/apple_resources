

- Core Media
- CMSyncProtocol
-  mightDrift(relativeTo:) 

Instance Method

# mightDrift(relativeTo:)

Returns a Boolean value that indicates whether it’s possible for the clock to drift relative to the input.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func mightDrift(relativeTo clockOrTimebase: T) -> Bool where T : CMSyncProtocol
```

**Required**

## Parameters 

`clockOrTimebase`  

The clock to compare to.

