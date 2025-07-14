

- HealthKit
- HKSourceRevision
-  init(source:version:) 

Initializer

# init(source:version:)

Initializes a new source revision object with the provided source and version information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    source: HKSource,
    version: String?
)
```

## Parameters 

`source`  

The source for a sample.

`version`  

A string that uniquely identifies the source’s version.

## Return Value

A newly initialized source revision object.

## Discussion

Use this method to create source revisions for use in queries. For more information, see HKPredicateKeyPathSourceRevision.

On iOS 9.0 or later, the system automatically creates a source revision for any samples saved to the HealthKit store. For earlier versions of iOS, the system only saves HKSource information. However, when these samples are retrieved on iOS 9.0 or later, the system creates a new source revision object for the sample. HealthKit uses the previously stored source information with a `nil`-valued version string.

## See Also

### Related Documentation

let HKSourceRevisionAnyVersion: String

A constant that matches any version.

### Creating Source Revision Objects

init(source: HKSource, version: String?, productType: String?, operatingSystemVersion: OperatingSystemVersion)

Initializes a new source revision object with the provided source, version, product type, and operating system.

