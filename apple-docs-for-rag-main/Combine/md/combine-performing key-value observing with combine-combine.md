

- Combine
-  Performing Key-Value Observing with Combine 

Article

# Performing Key-Value Observing with Combine

Expose KVO changes with a Combine publisher.

## Overview

Several frameworks use key-value observing to notify your app of asynchronous changes. By converting your use of KVO from callbacks and closures to Combine, you can make your code more elegant and maintainable.

### Monitoring Changes with KVO

In the following example, the type `UserInfo` supports KVO for its `lastLogin` property, as described in Using Key-Value Observing in Swift. The viewDidLoad() method uses the `observe(_:options:changeHandler:)` method to set up a closure that handles any change to the property. The closure receives an NSKeyValueObservedChange object that describes the change event, retrieves the newValue property, and prints it. The viewDidAppear(_:) method changes the value, which calls the closure and prints the message.

```
class UserInfo: NSObject {
    @objc dynamic var lastLogin: Date = Date(timeIntervalSince1970: 0)
}
@objc var userInfo = UserInfo()
var observation: NSKeyValueObservation?

override func viewDidLoad() {
    super.viewDidLoad()
    observation = observe(\.userInfo.lastLogin, options: [.new]) { object, change in
        print ("lastLogin now \(change.newValue!).")
    }
}

override func viewDidAppear(_ animated: Bool) {
    super.viewDidAppear(animated)
    userInfo.lastLogin = Date()
}
```

### Converting KVO Code to Use Combine

To convert KVO code to Combine, replace the `observe(_:options:changeHandler:)` method with an NSObject.KeyValueObservingPublisher. You get an instance of this publisher by calling `publisher(for:)` on the parent object, as shown in the following example’s viewDidLoad() method:

```
class UserInfo: NSObject {
    @objc dynamic var lastLogin: Date = Date(timeIntervalSince1970: 0)
}
@objc var userInfo = UserInfo()
var cancellable: Cancellable?

override func viewDidLoad() {
    super.viewDidLoad()
    cancellable = userInfo.publisher(for: \.lastLogin)
        .sink() { date in print ("lastLogin now \(date).") }
}

override func viewDidAppear(_ animated: Bool) {
    super.viewDidAppear(animated)
    userInfo.lastLogin = Date()
}
```

The KVO publisher produces elements of the observed type — in this case, Date — rather than NSKeyValueObservedChange. This saves you a step, because you don’t have to unpack the newValue from the change object, as in the first example.

## See Also

### Combine Migration

Routing Notifications to Combine Subscribers

Deliver notifications to subscribers by using notification centers’ publishers.

Replacing Foundation Timers with Timer Publishers

Publish elements periodically by using a timer.

Using Combine for Your App’s Asynchronous Code

Apply common patterns to migrate your closure-based, event-handling code.

