

- Core Text
- CTFontDescriptorMatchingState
-  CTFontDescriptorMatchingState.willBeginQuerying 

Case

# CTFontDescriptorMatchingState.willBeginQuerying

A state that indicates communication with the server is about to begin.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case willBeginQuerying
```

## Discussion

This state is skipped if unnecessary.

## See Also

### Constants

case didBegin

A state that indicates matching is about to begin.

case didFinish

A state that indicates matching is done.

case stalled

A state that indicates that matching is stalled, such as while waiting for a server response.

case willBeginDownloading

A state that indicates downloading is about to begin.

case downloading

A state that indicates downloading is in progress.

case didFinishDownloading

A state that indicates downloading is done.

case didMatch

A state that indicates the font descriptor match is successful.

case didFailWithError

A state that indicates an error.

