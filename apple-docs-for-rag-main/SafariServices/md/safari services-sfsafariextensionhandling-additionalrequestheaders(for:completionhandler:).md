

- Safari Services
- SFSafariExtensionHandling
-  additionalRequestHeaders(for:completionHandler:) 

Instance Method

# additionalRequestHeaders(for:completionHandler:)

macOS 10.13.4+

``` source
optional func additionalRequestHeaders(
    for url: URL,
    completionHandler: @escaping ([String : String]?) -> Void
)
```

``` source
optional func additionalRequestHeaders(for url: URL) async -> [String : String]?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func additionalRequestHeaders(for url: URL) async -> [String : String]?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

