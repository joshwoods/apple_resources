

- Core Data
- NSPersistentStore
- NSPersistentStore.StoreType
-  xml 

Type Property

# xml

A store that reads from and writes to a persistent XML file.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
static let xml: NSPersistentStore.StoreType
```

## Discussion

An XML store is atomic, which means Core Data reads and writes the file in its entirety. This behavior is different from a sqlite store, which you can partially modify.

## See Also

### Store Types

static let binary: NSPersistentStore.StoreType

A store that reads from and writes to a persistent binary file.

static let inMemory: NSPersistentStore.StoreType

An ephemeral store that reads from and writes to memory only.

static let sqlite: NSPersistentStore.StoreType

A store that reads from and writes to a persistent SQLite database.

