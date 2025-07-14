

- Core Data
- Core Data stack
- NSManagedObjectContext
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated type methods

class func new() -> SelfDeprecated

### Deprecated instance methods

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

convenience init()Deprecated

func lock()

Attempts to acquire a lock on the context.

Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

func unlock()

Relinquishes a previously acquired lock.

Deprecated

