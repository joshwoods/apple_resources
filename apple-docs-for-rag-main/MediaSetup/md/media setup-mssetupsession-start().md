

- Media Setup
- MSSetupSession
-  start() 

Instance Method

# start()

Initiates the service configuration process and sends the account details of the streaming media service to the user’s HomePod speakers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func start() throws
```

## See Also

### Presenting the Configuration View

var presentationContext: (any MSAuthenticationPresentationContext)?

A delegate that provides media setup display information to the system.

protocol MSAuthenticationPresentationContext

A protocol that provides media setup display information to the system.

