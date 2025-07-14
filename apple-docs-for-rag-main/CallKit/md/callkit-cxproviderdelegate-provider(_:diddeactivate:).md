

- CallKit
- CXProviderDelegate
-  provider(\_:didDeactivate:) 

Instance Method

# provider(\_:didDeactivate:)

Called when the provider’s audio session is deactivated.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
optional func provider(
    _ provider: CXProvider,
    didDeactivate audioSession: AVAudioSession
)
```

## Parameters 

`provider`  

The telephony provider.

`audioSession`  

The audio session that was deactivated.

## See Also

### Handling Changes to Audio Session Activation State

func provider(CXProvider, didActivate: AVAudioSession)

Called when the provider’s audio session is activated.

