

- WebKit
- WKWebsiteDataStore
-  removeData(ofTypes:modifiedSince:completionHandler:) 

Instance Method

# removeData(ofTypes:modifiedSince:completionHandler:)

Removes website data that changed after the specified date.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    modifiedSince date: Date,
    completionHandler: @escaping @MainActor () -> Void
)
```

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    modifiedSince date: Date
) async
```

## Parameters 

`dataTypes`  

The website data types to remove.

`date`  

The target date for the data removal. The data store removes data that a website changed after this date.

`completionHandler`  

The completion handler block to execute asynchronously after the web view removes the specified data. This block has no return value and takes no parameters.

## Discussion

This method removes the specified data type from all records, but only if a website modified the record’s data after the specified `date`.

## See Also

### Removing specific types of data

func removeData(ofTypes: Set&lt;String>, for: [WKWebsiteDataRecord], completionHandler: () -> Void)

Removes the specified types of website data from one or more data records.

