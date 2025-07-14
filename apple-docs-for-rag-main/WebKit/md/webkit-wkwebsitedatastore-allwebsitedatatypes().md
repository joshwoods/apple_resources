

- WebKit
- WKWebsiteDataStore
-  allWebsiteDataTypes() 

Type Method

# allWebsiteDataTypes()

Returns the set of all the available data types.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class func allWebsiteDataTypes() -> Set
```

## Discussion

Potential values in the set are WKWebsiteDataRecord constants.

## See Also

### Retrieving specific types of data

func fetchDataRecords(ofTypes: Set&lt;String>, completionHandler: ([WKWebsiteDataRecord]) -> Void)

Fetches the specified types of records from the data store.

