

- Media Setup
-  MSAuthenticationPresentationContext 

Protocol

# MSAuthenticationPresentationContext

A protocol that provides media setup display information to the system.

iOS 14.0+iPadOS 14.0+Mac Catalyst 15.4+visionOS 1.0+

``` source
protocol MSAuthenticationPresentationContext : NSObjectProtocol
```

## Topics

### Displaying the Media Setup View

func presentationAnchor() -> MSPresentationAnchor?

A window that presents the system’s HomePod configuration view to the user.

**Required**

typealias MSPresentationAnchor

A window that presents a Media Setup configuration view.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Presenting the Configuration View

var presentationContext: (any MSAuthenticationPresentationContext)?

A delegate that provides media setup display information to the system.

func start() throws

Initiates the service configuration process and sends the account details of the streaming media service to the user’s HomePod speakers.

