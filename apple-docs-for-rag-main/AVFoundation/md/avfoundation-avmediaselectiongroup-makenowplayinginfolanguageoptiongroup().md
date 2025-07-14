

- AVFoundation
- AVMediaSelectionGroup
-  makeNowPlayingInfoLanguageOptionGroup() 

Instance Method

# makeNowPlayingInfoLanguageOptionGroup()

Creates a language option group from the media selection group.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func makeNowPlayingInfoLanguageOptionGroup() -> MPNowPlayingInfoLanguageOptionGroup
```

## Return Value

The new language option group.

## Discussion

Any option from AVMediaSelectionOption in the AVMediaSelectionGroup not representing an audible or legible selection option is ignored.

