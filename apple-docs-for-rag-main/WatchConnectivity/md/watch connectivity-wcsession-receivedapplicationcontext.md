

- Watch Connectivity
- WCSession
-  receivedApplicationContext 

Instance Property

# receivedApplicationContext

A dictionary containing the last update data received from a paired and active device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
var receivedApplicationContext: [String : Any] { get }
```

## Discussion

Use this method to access the most recently received update dictionary. The session object also sends a newly arrived dictionary to the session(_:didReceiveApplicationContext:) method of its delegate.

## See Also

### Managing Background Updates

func updateApplicationContext([String : Any]) throws

Sends a dictionary of values that a paired and active device can use to synchronize its state.

var applicationContext: [String : Any]

The most recent contextual data sent to the paired and active device.

