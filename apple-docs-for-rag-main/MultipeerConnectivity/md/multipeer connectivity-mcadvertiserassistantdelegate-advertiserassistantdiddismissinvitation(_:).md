

- Multipeer Connectivity
- MCAdvertiserAssistantDelegate
-  advertiserAssistantDidDismissInvitation(\_:) 

Instance Method

# advertiserAssistantDidDismissInvitation(\_:)

Indicates that the advertiser assistant finished showing the invitation to the user.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
optional func advertiserAssistantDidDismissInvitation(_ advertiserAssistant: MCAdvertiserAssistant)
```

## Parameters 

`advertiserAssistant`  

The advertiser assistant that finished showing an invitation.

## Discussion

This call tells your app to resume any activity that it stopped doing while the invitation was onscreen. For example, it might resume computationally intensive UI updates for views that are no longer hidden by the invitation.

## See Also

### Advertiser Assistant Delegate Methods

func advertiserAssistantWillPresentInvitation(MCAdvertiserAssistant)

Indicates that the advertiser assistant is about to present an invitation to the user.

