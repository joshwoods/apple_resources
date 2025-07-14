

- Authentication Services
-  ASSettingsHelper 

Class

# ASSettingsHelper

A class that opens Settings and navigates to the settings for configuring credential providers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class ASSettingsHelper
```

## Topics

### Opening the Settings app

class func openCredentialProviderAppSettings(completionHandler: (((any Error)?) -> Void)?)

Open the Settings app and navigate to the AutoFill provider settings.

class func openVerificationCodeAppSettings(completionHandler: (((any Error)?) -> Void)?)

Open the Settings app and navigate to the verification code provider settings.

### Type Methods

class func requestToTurnOnCredentialProviderExtension(completionHandler: (Bool) -> Void)

Call this method from your containing app to request to turn on a contained Credential Provider Extension. If the extension is not currently enabled, a prompt will be shown to allow it to be turned on. The completion handler is called with YES or NO depending on whether the credential provider is enabled. You need to wait 10 seconds in order to make additional request to this API.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

