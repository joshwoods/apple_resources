

- Safari Services
- SFSafariExtension
-  getBaseURI(completionHandler:) 

Type Method

# getBaseURI(completionHandler:)

macOS 10.14.4+

``` source
class func getBaseURI(completionHandler: @escaping (URL?) -> Void)
```

``` source
class func baseURI() async -> URL?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func baseURI() async -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

