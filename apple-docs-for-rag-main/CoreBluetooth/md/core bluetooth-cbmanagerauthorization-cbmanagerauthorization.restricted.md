

- Core Bluetooth
- CBManagerAuthorization
-  CBManagerAuthorization.restricted 

Case

# CBManagerAuthorization.restricted

A state that indicates this app isn’t authorized to use Bluetooth.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case restricted
```

## Discussion

In this state, the user can’t change the Bluetooth authorization status, possibly due to active restrictions such as parental controls.

## See Also

### Authorization States

case allowedAlways

A state that indicates the user has authorized Bluetooth at any time.

case denied

A state that indicates the user explicitly denied Bluetooth access for this app.

case notDetermined

A state that indicates the user has yet to authorize Bluetooth for this app.

