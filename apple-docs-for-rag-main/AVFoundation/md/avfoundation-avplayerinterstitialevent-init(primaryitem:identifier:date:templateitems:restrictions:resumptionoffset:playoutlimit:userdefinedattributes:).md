

- AVFoundation
- AVPlayerInterstitialEvent
-  init(primaryItem:identifier:date:templateItems:restrictions:resumptionOffset:playoutLimit:userDefinedAttributes:) 

Initializer

# init(primaryItem:identifier:date:templateItems:restrictions:resumptionOffset:playoutLimit:userDefinedAttributes:)

Creates an interstitial event, with user-defined attributes, for the specified date.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    primaryItem: AVPlayerItem,
    identifier: String?,
    date: Date,
    templateItems: [AVPlayerItem],
    restrictions: AVPlayerInterstitialEvent.Restrictions = [],
    resumptionOffset: CMTime = .indefinite,
    playoutLimit: CMTime = .invalid,
    userDefinedAttributes: [String : Any] = [:]
)
```

## Parameters 

`primaryItem`  

The player item that represents the primary content. The item must contain an AVAsset that provides intrinsic mappings from its timeline to real-time dates.

`identifier`  

An external identifier for the event.

`date`  

A date within the date range of the primary item that playback of interstitial content begins.

`templateItems`  

An array of player item configurations to use as templates for player items that play interstitial content.

`restrictions`  

Restrictions on access to playback controls during the event.

`resumptionOffset`  

The time offset for resuming playback of the primary content after interstitial content finishes. You can specify a definite time, or specify indefinite to indicate that the effective resumption time offset needs to align with time elapsed during interstitial playback.

`playoutLimit`  

The time offset from the beginning of the interstitial when interstitial playback needs to end, if interstitial assets are longer. Pass a positive numeric value, or invalid to indicate no play out limit.

`userDefinedAttributes`  

Custom attributes to add to the event.

## See Also

### Creating an event

convenience init(primaryItem: AVPlayerItem, time: CMTime)

Creates an interstitial event for the specified time.

convenience init(primaryItem: AVPlayerItem, date: Date)

Creates an interstitial event for the specified date.

convenience init(primaryItem: AVPlayerItem, identifier: String?, time: CMTime, templateItems: [AVPlayerItem], restrictions: AVPlayerInterstitialEvent.Restrictions, resumptionOffset: CMTime, playoutLimit: CMTime, userDefinedAttributes: [String : Any])

Creates an interstitial event, with user-defined attributes, for the specified time.

