

- SecureElementCredential
-  CredentialSessionWindowSceneDelegate 

Protocol

# CredentialSessionWindowSceneDelegate

A protocol to notify a UIKit scene that a credential session event occurred.

SecureElementCredentialUIKitiOS 17.4+iPadOS 17.4+

``` source
protocol CredentialSessionWindowSceneDelegate
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

Warning

Don’t import SwiftUI in any files that refer to symbols defined in this protocol. Importing SwiftUI and UIKit in the same file results in ambiguity during compilation.

## Topics

### Handling events

func windowScene(UIWindowScene, didReceiveCredentialSessionWindowSceneEvent: CredentialSessionWindowSceneEvent)

Informs your app that a credential session event initiated a UIKit scene creation.

**Required**

enum CredentialSessionWindowSceneEvent

An event that a credential session sends to a UIKit scene.

