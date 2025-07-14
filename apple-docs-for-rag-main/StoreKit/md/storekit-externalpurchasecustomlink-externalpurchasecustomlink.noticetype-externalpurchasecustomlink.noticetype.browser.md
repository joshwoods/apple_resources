

- StoreKit
- ExternalPurchaseCustomLink
- ExternalPurchaseCustomLink.NoticeType
-  ExternalPurchaseCustomLink.NoticeType.browser 

Case

# ExternalPurchaseCustomLink.NoticeType.browser

A notice type that indicates you display external purchases in a destination outside of the app, which can be an alternative marketplace, another app, or a website.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
case browser
```

## Discussion

After displaying a notice with this notice type using showNotice(type:), if the customer chooses to continue, the app goes to the background and presents external purchases in a destination outside of the app. The destination can be an alternative app marketplace, another app, or a website.

## See Also

### Getting notice types

case withinApp

A notice type that indicates that you display the destination in a web view within the app.

