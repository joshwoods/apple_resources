

- Watch Connectivity
- WCSession
-  applicationContext 

Instance Property

# applicationContext

The most recent contextual data sent to the paired and active device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
var applicationContext: [String : Any] { get }
```

## Discussion

After calling the updateApplicationContext(_:) method, the session object places a copy of your dictionary in this property so that you can determine what data you last sent to the counterpart.

## See Also

### Managing Background Updates

func updateApplicationContext([String : Any]) throws

Sends a dictionary of values that a paired and active device can use to synchronize its state.

var receivedApplicationContext: [String : Any]

A dictionary containing the last update data received from a paired and active device.

