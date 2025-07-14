

- Core Data
-  NSFetchedResultsSectionInfo 

Protocol

# NSFetchedResultsSectionInfo

A protocol that defines the interface for section objects vended by a fetched results controller.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol NSFetchedResultsSectionInfo
```

## Topics

### Accessing Objects

var numberOfObjects: Int

The number of objects (rows) in the section.

**Required**

var objects: [Any]?

The array of objects in the section.

**Required**

### Accessing the Name and Title

var name: String

The name of the section.

**Required**

var indexTitle: String?

The index title of the section.

**Required**

## See Also

### Responding to Changes

protocol NSFetchedResultsControllerDelegate

A delegate protocol that describes the methods that the associated fetched results controller calls when the fetch results change.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

enum NSFetchedResultsChangeType

Constants that specify the possible types of changes that are reported.

