

- OSLog
- OSLogStore
-  local() 

Type Method

# local()

Creates a log store representing the Mac’s local store.

macOS 10.15+

``` source
class func local() throws -> Self
```

## Discussion

Gaining access to the local unified logging system requires permission from the system. The caller must be run by an admin account and have the `com.apple.logging.local-store` entitlement.

## See Also

### Creating Log Stores

convenience init(url: URL) throws

Creates a log store based on a log archive.

