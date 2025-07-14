

- CallKit
- CXProviderDelegate
-  provider(\_:didActivate:) 

Instance Method

# provider(\_:didActivate:)

Called when the provider’s audio session is activated.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
optional func provider(
    _ provider: CXProvider,
    didActivate audioSession: AVAudioSession
)
```

## Parameters 

`provider`  

The telephony provider.

`audioSession`  

The audio session that was activated.

## See Also

### Handling Changes to Audio Session Activation State

func provider(CXProvider, didDeactivate: AVAudioSession)

Called when the provider’s audio session is deactivated.

