

- Multipeer Connectivity
- MCAdvertiserAssistantDelegate
-  advertiserAssistantWillPresentInvitation(\_:) 

Instance Method

# advertiserAssistantWillPresentInvitation(\_:)

Indicates that the advertiser assistant is about to present an invitation to the user.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
optional func advertiserAssistantWillPresentInvitation(_ advertiserAssistant: MCAdvertiserAssistant)
```

## Parameters 

`advertiserAssistant`  

The advertiser assistant that is about to present an invitation to the user.

## Discussion

This call is intended to allow your app to prepare for an invitation that will be presented to the user. For example, your app might stop performing computationally intensive UI updates for views that will be hidden by the invitation.

## See Also

### Advertiser Assistant Delegate Methods

func advertiserAssistantDidDismissInvitation(MCAdvertiserAssistant)

Indicates that the advertiser assistant finished showing the invitation to the user.

