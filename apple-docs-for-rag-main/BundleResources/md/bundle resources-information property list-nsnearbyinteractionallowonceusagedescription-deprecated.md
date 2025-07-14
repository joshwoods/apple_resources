

- Bundle Resources
- Information Property List
-  NSNearbyInteractionAllowOnceUsageDescription Deprecated

Property List Key

# NSNearbyInteractionAllowOnceUsageDescription

A one-time request for user permission to begin an interaction session with nearby devices.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0Deprecated

## Details 

Name  
Privacy - Nearby Interaction Allow Once Usage Description

Type  

string

## Discussion

Warning

Define this property in the `Info.plist` only for apps that deploy to iOS 14. NSNearbyInteractionUsageDescription replaces this property in iOS 15 and later.

Before an app starts an interaction session, the system requests permission to share the user’s relative distance and direction with a nearby peer. The framework presents a prompt that displays the value of this key contained in your project’s `Info.plist`. Define text that explains your interaction session’s purpose to the user. For more information, see Initiating and maintaining a session.

## See Also

### Networking

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

**Name:** Privacy - Local Network Usage Description

NSNearbyInteractionUsageDescription

A request for user permission to begin an interaction session with nearby devices.

**Name:** Privacy - Nearby Interaction Usage Description

