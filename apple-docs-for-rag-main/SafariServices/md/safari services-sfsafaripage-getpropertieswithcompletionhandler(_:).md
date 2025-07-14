

- Safari Services
- SFSafariPage
-  getPropertiesWithCompletionHandler(\_:) 

Instance Method

# getPropertiesWithCompletionHandler(\_:)

Retrieves the properties of the webpage.

macOS 10.12+

``` source
func getPropertiesWithCompletionHandler(_ completionHandler: @escaping (SFSafariPageProperties?) -> Void)
```

``` source
func properties() async -> SFSafariPageProperties?
```

## Parameters 

`completionHandler`  

A block to call when the properties object is returned.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func properties() async -> SFSafariPageProperties?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If the extension cannot access the page—for example, the extension has web access permissions set to `None` in the Info.plist—the properties object passed to the completion handler is `nil`. See SFSafariPageProperties.

