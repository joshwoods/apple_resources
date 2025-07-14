

- ARKit
- ARAppClipCodeAnchor
-  url 

Instance Property

# url

The URL encoded in an App Clip Code.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
var url: URL? { get }
```

## Discussion

To enable users to decode your App Clip code’s URL from an App Clip or within an AR app, associate your App Clip with its App Clip Code(s) in App Store Connect; for more information, see set up an App Clip experience. Because each App Clip Code belongs to a specific App Clip experience, you can decode an App Clip Code URL in a full app’s AR experience only after first providing an accompanying App Clip.

This property is `nil` by default. The framework sets a value for this property when urlDecodingState is ARAppClipCodeAnchor.URLDecodingState.decoded. This property remains `nil` for App Clip Codes that belong to another App Clip experience or development team.

### Distribute Your App and App Clip for Testing

Although you can launch an App Clip from the camera after creating an App Clip local experience, ARKit checks the App Clip experience registry in App Store Connect to determine if your App Clip associates to a particular App Clip Code URL. When ARKit confirms that an App Clip Code in the physical environment belongs to your App Clip experience, the framework sets the value of this property.

After setting up an App Clip experience, distribute your app to testers; for more information, see Testing the launch experience of your App Clip.

## See Also

### Decoding the URL

var urlDecodingState: ARAppClipCodeAnchor.URLDecodingState

A state that indicates the process of decoding an App Clip Code URL.

enum URLDecodingState

The states in the process of decoding an App Clip code URL.

