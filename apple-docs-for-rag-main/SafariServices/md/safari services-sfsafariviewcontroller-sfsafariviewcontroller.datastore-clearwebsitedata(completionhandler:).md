

- Safari Services
- SFSafariViewController
- SFSafariViewController.DataStore
-  clearWebsiteData(completionHandler:) 

Instance Method

# clearWebsiteData(completionHandler:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func clearWebsiteData(completionHandler completion: (() -> Void)? = nil)
```

``` source
func clearWebsiteData() async
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func clearWebsiteData() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

