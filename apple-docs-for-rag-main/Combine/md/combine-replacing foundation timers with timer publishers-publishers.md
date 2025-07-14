

- Combine
-  Replacing Foundation Timers with Timer Publishers 

Article

# Replacing Foundation Timers with Timer Publishers

Publish elements periodically by using a timer.

## Overview

If your app uses Foundation’s Timer class to repeatedly receive a callback or invoke a closure on a specified interval, you can convert these instances to Combine to simplify your code.

### Performing Periodic Work with a Timer

Consider the following snippet, which uses scheduledTimer(withTimeInterval:repeats:block:) to update the `lastUpdated` property of a data model once a second, on a specific dispatch queue:

```
var timer: Timer?
override func viewDidLoad() {
    super.viewDidLoad()
    timer = Timer.scheduledTimer(withTimeInterval: 1, repeats: true) { _ in
        self.myDispatchQueue.async() {
            self.myDataModel.lastUpdated = Date()
        }
    }
}
```

### Converting to a Timer Publisher

To migrate this code to Combine, replace the Timer that is returned by scheduledTimer(withTimeInterval:repeats:block:) with a Timer.TimerPublisher. You create this publisher with the Timer method publish(every:tolerance:on:in:options:). Every time the underyling Timer fires, the publisher emits a new Date that represents the instant the timer fired. You then apply Combine operators to the Date, eventually connecting the publisher to a subscriber like sink(receiveValue:) or assign(to:on:).

Tip

Because Timer.TimerPublisher conforms to the ConnectablePublisher protocol, it won’t produce elements until you explicitly connect to it. Do this by either calling connect(), or using an autoconnect() operator to connect automatically when a subscriber attaches.

The next example shows how to use a Timer.TimerPublisher to replace the previous example. It uses Combine’s operators to perform the tasks that were in the previous example’s closure:

```
var cancellable: Cancellable?
override func viewDidLoad() {
    super.viewDidLoad()
    cancellable = Timer.publish(every: 1, on: .main, in: .default)
        .autoconnect()
        .receive(on: myDispatchQueue)
        .assign(to: \.lastUpdated, on: myDataModel)
}
```

In this example, Combine operators replace all the behavior inside the closure of the earlier example:

- The receive(on:options:) operator ensures that its subsequent operators run on the specified dispatch queue. This replaces the `async()` call from before.

- The assign(to:on:) operator updates the data model, by using a key path to set the `lastUpdate` property.

Another advantage you’ll find when using Combine to simplify your code is that the Timer.TimerPublisher produces new Date instances as its output type. The first example’s closure receives the Timer itself as its parameter, so it has to create new Date instances manually.

## See Also

### Combine Migration

Routing Notifications to Combine Subscribers

Deliver notifications to subscribers by using notification centers’ publishers.

Performing Key-Value Observing with Combine

Expose KVO changes with a Combine publisher.

Using Combine for Your App’s Asynchronous Code

Apply common patterns to migrate your closure-based, event-handling code.

