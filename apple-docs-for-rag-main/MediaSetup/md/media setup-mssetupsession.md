

- Media Setup
-  MSSetupSession 

Class

# MSSetupSession

An object that manages the transfer of configuration information between your app, the system, your media service, and HomePod speakers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MSSetupSession
```

## Overview

An `MSSetupSession` object guides the user through connecting HomePod speakers in their home to your media service. When your iOS app calls start(), the session displays a setup view in the window you provide in presentationAnchor(). The session embeds your app icon and the serviceName you provide into this setup view.

After the user confirms the setup by tapping the “Use in Home” button, the system requests an OAuth token from your authentication service and shares the token with HomePod speakers in the user’s home.

## Topics

### Preparing the Configuration View

init(serviceAccount: MSServiceAccount)

Creates a new session.

var account: MSServiceAccount

The streaming media service account for the session to configure.

### Presenting the Configuration View

var presentationContext: (any MSAuthenticationPresentationContext)?

A delegate that provides media setup display information to the system.

protocol MSAuthenticationPresentationContext

A protocol that provides media setup display information to the system.

func start() throws

Initiates the service configuration process and sends the account details of the streaming media service to the user’s HomePod speakers.

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

## See Also

### HomePod Configuration

class MSServiceAccount

Account details for accessing a streaming media service.

