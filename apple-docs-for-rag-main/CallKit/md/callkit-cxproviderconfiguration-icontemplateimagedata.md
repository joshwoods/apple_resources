

- CallKit
- CXProviderConfiguration
-  iconTemplateImageData 

Instance Property

# iconTemplateImageData

The PNG data for the icon image to be displayed for the provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
var iconTemplateImageData: Data? { get set }
```

## Discussion

The icon image should be a square with side length of 40 points. The alpha channel of the image is used to create a white image mask, which is used in the system native in-call UI for the button which takes the user from this system UI to the 3rd-party app.

## See Also

### Configuring Native Call UI

var localizedName: String?

The localized name of the provider.

Deprecated

var ringtoneSound: String?

The name of the sound resource in the app bundle to be used for the provider ringtone.

