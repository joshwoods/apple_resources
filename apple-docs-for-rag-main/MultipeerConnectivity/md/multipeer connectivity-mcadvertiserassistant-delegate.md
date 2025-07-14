

- Multipeer Connectivity
- MCAdvertiserAssistant
-  delegate 

Instance Property

# delegate

The delegate object that handles advertising-assistant-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any MCAdvertiserAssistantDelegate)? { get set }
```

## See Also

### Initializing and Configuring

init(serviceType: String, discoveryInfo: [String : String]?, session: MCSession)

Initializes an advertiser assistant object.

var session: MCSession

The session into which new peers are added after accepting an invitation.

var discoveryInfo: [String : String]?

The `info` dictionary that was passed when this object was initialized.

var serviceType: String

The service type that your app is advertising.

