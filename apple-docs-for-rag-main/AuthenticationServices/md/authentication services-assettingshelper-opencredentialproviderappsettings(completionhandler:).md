

- Authentication Services
- ASSettingsHelper
-  openCredentialProviderAppSettings(completionHandler:) 

Type Method

# openCredentialProviderAppSettings(completionHandler:)

Open the Settings app and navigate to the AutoFill provider settings.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class func openCredentialProviderAppSettings(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
class func openCredentialProviderAppSettings() async throws
```

## Parameters 

`completionHandler`  

An optional block that the system calls on completion.

## See Also

### Opening the Settings app

class func openVerificationCodeAppSettings(completionHandler: (((any Error)?) -> Void)?)

Open the Settings app and navigate to the verification code provider settings.

