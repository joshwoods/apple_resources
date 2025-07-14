

- UIKit
- UITextInputMode
-  activeInputModes 

Type Property

# activeInputModes

The active text-input modes.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var activeInputModes: [UITextInputMode] { get }
```

## Discussion

Each element in the array is an instance of UITextInputMode. Returns an empty array if no such instances have been set by the text input system.

Important

This API has the potential of being misused to access device signals to try to identify the device or user, also known as fingerprinting. Regardless of whether a user gives your app permission to track, fingerprinting is not allowed. When you use this API in your app or third-party SDK (an SDK not provided by Apple), declare your usage and the reason for using the API in your app or third-party SDK’s `PrivacyInfo.xcprivacy` file. For more information, including the list of valid reasons for using the API, see Describing use of required reason API.

