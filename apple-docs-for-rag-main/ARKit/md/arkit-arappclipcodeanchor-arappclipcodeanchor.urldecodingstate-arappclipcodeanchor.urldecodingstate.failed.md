

- ARKit
- ARAppClipCodeAnchor
- ARAppClipCodeAnchor.URLDecodingState
-  ARAppClipCodeAnchor.URLDecodingState.failed 

Case

# ARAppClipCodeAnchor.URLDecodingState.failed

A state that indicates the failure to decode an App Clip Code’s URL.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
case failed
```

## Discussion

The decoding of an App Clip Code URL fails under these circumstances:

- The full app or App Clip is missing the associated-domains entitlement from its code signature.

- The host of the resource identified by the App Clip Code URL doesn’t vend an Apple App Site Association (AASA) file.

- The AASA file hosted at the App Clip Code URL’s domain lacks the App Clip’s fully-qualified application identifier.

- The App Clip Code is not associated to the App Clip in an App Clip experience in App Store Connect.

For more information, see Configuring the launch experience of your App Clip.

## See Also

### States

case decoded

A state that indicates the completed decoding of an App Clip Code URL.

case decoding

A state that indicates the continuing process of decoding an App Clip Code’s URL.

