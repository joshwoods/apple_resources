

- Core Bluetooth
- CBManager
-  authorization 

Type Property

# authorization

The current authorization status for using Bluetooth.

iOS 13.1+iPadOS 13.1+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var authorization: CBManagerAuthorization { get }
```

## Discussion

Check this property in your implementation of the delegate methods centralManagerDidUpdateState(_:) and peripheralManagerDidUpdateState(_:) to determine whether your app can use Core Bluetooth. You can also use it to check the app’s authorization status before creating a CBManager instance.

The initial value of this property is CBManagerAuthorization.notDetermined.

## See Also

### Determining Authorization State

enum CBManagerAuthorization

The current authorization state of a Core Bluetooth manager.

