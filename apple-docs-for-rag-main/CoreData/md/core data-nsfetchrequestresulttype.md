

- Core Data
-  NSFetchRequestResultType 

Structure

# NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct NSFetchRequestResultType
```

## Overview

These constants are used by resultType.

## Topics

### Result Types

static var managedObjectResultType: NSFetchRequestResultType

The request returns managed objects.

static var managedObjectIDResultType: NSFetchRequestResultType

The request returns managed object IDs.

static var dictionaryResultType: NSFetchRequestResultType

The request returns dictionaries.

static var countResultType: NSFetchRequestResultType

The request returns the count of the objects that match the request.

### Initializers

init(rawValue: UInt)

Creates a fetch request result type using the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing the Fetch Request’s Entity

init()

Creates a new fetch request.

convenience init(entityName: String)

Initializes a fetch request configured with a given entity name.

var entityName: String?

The name of the entity the request is configured to fetch.

var entity: NSEntityDescription?

The entity specified for the fetch request.

var includesSubentities: Bool

A Boolean value that indicates whether the fetch request includes subentities in the results.

