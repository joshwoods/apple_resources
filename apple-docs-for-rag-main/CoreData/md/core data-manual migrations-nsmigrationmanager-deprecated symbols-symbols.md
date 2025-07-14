

- Core Data
- Manual migrations
- NSMigrationManager
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated Methods

func migrateStore(from: URL, sourceType: String, options: [AnyHashable : Any]?, with: NSMappingModel?, toDestinationURL: URL, destinationType: String, destinationOptions: [AnyHashable : Any]?) throws

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

Deprecated

