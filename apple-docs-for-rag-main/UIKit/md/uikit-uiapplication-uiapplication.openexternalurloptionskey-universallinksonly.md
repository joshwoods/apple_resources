

- UIKit
- UIApplication
- UIApplication.OpenExternalURLOptionsKey
-  universalLinksOnly 

Type Property

# universalLinksOnly

URLs must be universal links and have an app configured to open them.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
static let universalLinksOnly: UIApplication.OpenExternalURLOptionsKey
```

## Discussion

When you include this key in the options dictionary of the open(_:options:completionHandler:) method, the method opens the URL only if the URL is a valid universal link and there is an installed app capable of opening that URL. The value of this key is an NSNumber object containing a Boolean value.

