

- MapKit
- MKMapItem
-  openMaps(with:launchOptions:completionHandler:) 

Type Method

# openMaps(with:launchOptions:completionHandler:)

Opens the Maps app using the specified map items and options.

macOS 14.4+

``` source
class func openMaps(
    with mapItems: [MKMapItem],
    launchOptions: [String : Any]? = nil,
    completionHandler completion: ((Bool) -> Void)? = nil
)
```

``` source
class func openMaps(
    with mapItems: [MKMapItem],
    launchOptions: [String : Any]? = nil
) async -> Bool
```

## Parameters 

`mapItems`  

An array of map items to open in the Maps app.

`launchOptions`  

A dictionary of launch options to pass to the Maps app.

`completion`  

A completion block the system calls that indicates whether the request was successful.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func openMaps(with mapItems: [MKMapItem], launchOptions: [String : Any]? = nil) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Launching the Maps app

class func openMaps(with: [MKMapItem], launchOptions: [String : Any]?) -> Bool

Opens the Maps app and displays the specified map items.

class func openMaps(with: [MKMapItem], launchOptions: [String : Any]?, from: UIScene?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app from a particular scene using the specified map items and options.

func openInMaps(launchOptions: [String : Any]?) -> Bool

Opens the Maps app and displays the map item.

func openInMaps(launchOptions: [String : Any]?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app and displays the map item.

func openInMaps(launchOptions: [String : Any]?, from: UIScene?, completionHandler: ((Bool) -> Void)?)

Opens the Maps app from a particular scene using the specified options.

