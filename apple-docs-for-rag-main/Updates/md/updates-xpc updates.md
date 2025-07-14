

- Updates
-  XPC updates 

Article

# XPC updates

Learn about important changes to XPC.

## Overview

Browse notable changes in XPC.

## March 2024

### Security

- Test whether the peer executable that communicates with your app over an XPC connection has an expected entitlement by calling xpc_connection_set_peer_entitlement_exists_requirement(_:_:), and whether it has a specific value for an entitlement by calling xpc_connection_set_peer_entitlement_matches_value_requirement(_:_:_:).

- Test whether the peer executable that communicates with your app over an XPC connection is an Apple platform binary with a given signing identifier by calling xpc_connection_set_peer_platform_identity_requirement(_:_:).

- Test whether your Apple Developer team signed the peer executable that communicates with your app over an XPC connection by calling xpc_connection_set_peer_team_identity_requirement(_:_:).

- Test whether the peer executable that communicates with your app over an XPC connection satisfies a lightweight code requirement by calling xpc_connection_set_peer_lightweight_code_requirement(_:_:).

## June 2023

- Create XPC services using native Swift syntax. Use XPCListener to create an XPC server that listens for messages from other processes. Use XPCSession to create clients that connect to servers and exchange messages.

- For C and Objective-C projects, use the corresponding xpc_listener_t and xpc_session_t APIs.

- In Xcode, use the updated XPC services target template to choose whether you want to use the high-level NSXPCConnection or the low-level `libXPC` APIs.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

