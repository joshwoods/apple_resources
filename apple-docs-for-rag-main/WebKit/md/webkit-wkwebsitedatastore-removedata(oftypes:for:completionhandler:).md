

- WebKit
- WKWebsiteDataStore
-  removeData(ofTypes:for:completionHandler:) 

Instance Method

# removeData(ofTypes:for:completionHandler:)

Removes the specified types of website data from one or more data records.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    for dataRecords: [WKWebsiteDataRecord],
    completionHandler: @escaping @MainActor () -> Void
)
```

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    for dataRecords: [WKWebsiteDataRecord]
) async
```

## Parameters 

`dataTypes`  

The website data types to remove from the records.

`dataRecords`  

The records that contain the data.

`completionHandler`  

The completion handler block to execute asynchronously after the web view removes the specified data. This block has no return value and takes no parameters.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func removeData(ofTypes dataTypes: Set, for dataRecords: [WKWebsiteDataRecord]) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Removing specific types of data

func removeData(ofTypes: Set&lt;String>, modifiedSince: Date, completionHandler: () -> Void)

Removes website data that changed after the specified date.

