

- SecureElementCredential
- CredentialSessionWindowSceneDelegate
-  windowScene(\_:didReceiveCredentialSessionWindowSceneEvent:) 

Instance Method

# windowScene(\_:didReceiveCredentialSessionWindowSceneEvent:)

Informs your app that a credential session event initiated a UIKit scene creation.

SecureElementCredentialUIKitiOS 17.4+iPadOS 17.4+

``` source
func windowScene(
    _ windowScene: UIWindowScene,
    didReceiveCredentialSessionWindowSceneEvent event: CredentialSessionWindowSceneEvent
)
```

**Required**

## Parameters 

`windowScene`  

The scene object connected to your app.

`event`  

The CredentialSessionWindowSceneEvent that initiated the new scene.

## See Also

### Handling events

enum CredentialSessionWindowSceneEvent

An event that a credential session sends to a UIKit scene.

