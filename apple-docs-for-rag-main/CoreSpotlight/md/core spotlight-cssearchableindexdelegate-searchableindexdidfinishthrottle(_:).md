

- Core Spotlight
- CSSearchableIndexDelegate
-  searchableIndexDidFinishThrottle(\_:) 

Instance Method

# searchableIndexDidFinishThrottle(\_:)

Tells the delegate that the index throttling has finished.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
optional func searchableIndexDidFinishThrottle(_ searchableIndex: CSSearchableIndex)
```

## Parameters 

`searchableIndex`  

The index that was throttled.

## Discussion

In some situations, such as when the device is using battery only, the system may throttle indexing to save power. You can implement this method to be notified when throttling is finished so that your app can resume its standard indexing behavior.

## See Also

### Getting information about indexing

func searchableIndexDidThrottle(CSSearchableIndex)

Tells the delegate that indexing is being throttled.

