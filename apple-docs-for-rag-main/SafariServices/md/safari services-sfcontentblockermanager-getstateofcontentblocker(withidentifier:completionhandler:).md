

- Safari Services
- SFContentBlockerManager
-  getStateOfContentBlocker(withIdentifier:completionHandler:) 

Type Method

# getStateOfContentBlocker(withIdentifier:completionHandler:)

Determines the state of your content blocker.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
class func getStateOfContentBlocker(
    withIdentifier identifier: String,
    completionHandler: @escaping (SFContentBlockerState?, (any Error)?) -> Void
)
```

``` source
class func stateOfContentBlocker(withIdentifier identifier: String) async throws -> SFContentBlockerState
```

## Parameters 

`identifier`  

The bundle identifier of your content blocker extension.

`completionHandler`  

The code block to invoke with the state of the content blocker.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func stateOfContentBlocker(withIdentifier identifier: String) async throws -> SFContentBlockerState
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The `state` parameter of the completion handler’s `SFContentBlockerState` contains the isEnabled property. If the content blocker is enabled, `state.isEnabled` is true; otherwise it’s false. See SFContentBlockerState.

