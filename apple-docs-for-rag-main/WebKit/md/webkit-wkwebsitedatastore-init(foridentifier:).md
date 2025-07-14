

- WebKit
- WKWebsiteDataStore
-  init(forIdentifier:) 

Initializer

# init(forIdentifier:)

Returns the persistent data store with the unique identifier you provide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
init(forIdentifier identifier: UUID)
```

## Parameters 

`identifier`  

An identifier that uniquely identifies a data store.

## Discussion

If the data store for the unique identifier you provide does not exist, the system creates and returns it. Use this method to get a data store for a profile.

This method throws an exception if the identifier is not valid.

## See Also

### Creating a data store object

class func `default`() -> WKWebsiteDataStore

Returns the default data store, which stores data persistently to disk.

class func nonPersistent() -> WKWebsiteDataStore

Creates a new data store object that stores website data in memory, and doesn’t write that data to disk.

