

- Bundle Resources
- Information Property List
-  NSNearbyInteractionUsageDescription 

Property List Key

# NSNearbyInteractionUsageDescription

A request for user permission to begin an interaction session with nearby devices.

iOS 15.0+iPadOS 15.0+watchOS 8.0+

## Details 

Name  
Privacy - Nearby Interaction Usage Description

Type  

string

## Discussion

This property defines localizable text that explains your interaction session’s purpose to the user.

Before an app starts an interaction session, the system checks whether the user agrees to share their relative distance and direction with a nearby peer. The first time the app runs, the framework presents a prompt that displays the value of this key contained in your project’s `Info.plist`. The system persists the user’s choice in Settings. After your app runs for the first time, it consults the user preference in Settings before it begins a new interaction session.

For more information, see Initiating and maintaining a session.

## See Also

### Networking

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

**Name:** Privacy - Local Network Usage Description

NSNearbyInteractionAllowOnceUsageDescription

A one-time request for user permission to begin an interaction session with nearby devices.

**Name:** Privacy - Nearby Interaction Allow Once Usage Description

Deprecated

