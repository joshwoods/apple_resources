

- Safari Services
- SFSafariTab
-  activate(completionHandler:) 

Instance Method

# activate(completionHandler:)

Activates the tab.

macOS 10.12+

``` source
func activate(completionHandler: (() -> Void)? = nil)
```

``` source
func activate() async
```

## Parameters 

`completionHandler`  

A block to call when the tab is activated.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func activate() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

