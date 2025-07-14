

- Core ML
- MLModelCollection
-  didChangeNotification Deprecated

Type Property

# didChangeNotification

The notification the framework sends when it receives an update to a model collection.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedvisionOS 1.0–1.1Deprecated

``` source
class let didChangeNotification: NSNotification.Name
```

Deprecated

Use Background Assets or URLSession instead.

## Discussion

Register your app to get notifications when a model collection update is available by calling addObserver(forName:object:queue:using:).

```
let center = NotificationCenter.default
var token: NSObjectProtocol?

token = center.addObserver(forName: MLModelCollection.didChangeNotification,
                           object: nil,
                           queue: nil) { [unowned self] note in
    guard let modelCollection = note.object as? MLModelCollection else {
        print("Model Collection notification's object is not a model collection")
        return
    }

    // Use updated model collection ...
    self.receivedUpdatedModelCollection(modelCollection)

    // Clean up notification registration.
    center.removeObserver(token!)
}
```

Typically, you register for model collection notifications when your app needs to use the newest models as soon as the collection is available. Your app can always get the newest model collection by calling beginAccessingModelCollectionWithIdentifier:completionHandler:.

