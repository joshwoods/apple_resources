

- Media Setup
- MSSetupSession
-  presentationContext 

Instance Property

# presentationContext

A delegate that provides media setup display information to the system.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
weak var presentationContext: (any MSAuthenticationPresentationContext)? { get set }
```

## See Also

### Presenting the Configuration View

protocol MSAuthenticationPresentationContext

A protocol that provides media setup display information to the system.

func start() throws

Initiates the service configuration process and sends the account details of the streaming media service to the user’s HomePod speakers.

