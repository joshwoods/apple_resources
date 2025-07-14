

- MapKit
- MKMapItem
-  openInMaps(launchOptions:completionHandler:) 

Instance Method

# openInMaps(launchOptions:completionHandler:)

Opens the Maps app and displays the map item.

macOS 14.4+

``` source
func openInMaps(
    launchOptions: [String : Any]? = nil,
    completionHandler completion: ((Bool) -> Void)? = nil
)
```

``` source
func openInMaps(launchOptions: [String : Any]? = nil) async -> Bool
```

## Parameters 

`launchOptions`  

A dictionary of launch options to pass to the Maps app.

`completion`  

A completion block the system calls that indicates whether the request was successful.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func openInMaps(launchOptions: [String : Any]? = nil) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Launching the Maps app

class func openMaps(with: [MKMapItem], launchOptions: [String : Any]?) -> Bool

Opens the Maps app and displays the specified map items.

class func openMaps(with: [MKMapItem], launchOptions: [String : Any]?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app using the specified map items and options.

class func openMaps(with: [MKMapItem], launchOptions: [String : Any]?, from: UIScene?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app from a particular scene using the specified map items and options.

func openInMaps(launchOptions: [String : Any]?) -> Bool

Opens the Maps app and displays the map item.

func openInMaps(launchOptions: [String : Any]?, from: UIScene?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app from a particular scene using the specified options.

