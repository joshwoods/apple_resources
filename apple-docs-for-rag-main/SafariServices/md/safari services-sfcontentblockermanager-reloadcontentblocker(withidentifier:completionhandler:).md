

- Safari Services
- SFContentBlockerManager
-  reloadContentBlocker(withIdentifier:completionHandler:) 

Type Method

# reloadContentBlocker(withIdentifier:completionHandler:)

Tells Safari to reload the specified extension’s content-blocking rules.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+

``` source
class func reloadContentBlocker(
    withIdentifier identifier: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func reloadContentBlocker(withIdentifier identifier: String) async throws
```

## Parameters 

`identifier`  

The bundle identifier of your content blocker extension.

`completionHandler`  

The code to run after the content-blocking rules are reloaded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func reloadContentBlocker(withIdentifier identifier: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method when your extension’s content-blocking rules change.

