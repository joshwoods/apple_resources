

- Core Spotlight
- CSSearchableIndexDelegate
-  searchableIndexDidThrottle(\_:) 

Instance Method

# searchableIndexDidThrottle(\_:)

Tells the delegate that indexing is being throttled.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
optional func searchableIndexDidThrottle(_ searchableIndex: CSSearchableIndex)
```

## Parameters 

`searchableIndex`  

The indexing that’s being throttled.

## Discussion

In some situations, such as when the device is using battery only, the system may throttle indexing to save power. You can implement this method to be notified of this situation so that you can respond by, for example, prioritizing the items to index.

## See Also

### Getting information about indexing

func searchableIndexDidFinishThrottle(CSSearchableIndex)

Tells the delegate that the index throttling has finished.

