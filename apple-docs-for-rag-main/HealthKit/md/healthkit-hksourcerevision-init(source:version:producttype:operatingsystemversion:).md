

- HealthKit
- HKSourceRevision
-  init(source:version:productType:operatingSystemVersion:) 

Initializer

# init(source:version:productType:operatingSystemVersion:)

Initializes a new source revision object with the provided source, version, product type, and operating system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    source: HKSource,
    version: String?,
    productType: String?,
    operatingSystemVersion: OperatingSystemVersion
)
```

## Parameters 

`source`  

The source for a sample.

`version`  

A string that uniquely identifies the source’s version.

`productType`  

A string that identifies the device used to save the sample.

`operatingSystemVersion`  

A string that identifies the operating system used to save the sample.

## Return Value

A newly initialized source revision object.

## Discussion

Use this method to create source revisions for use in queries. For more information, see HKPredicateKeyPathSourceRevision.

## See Also

### Related Documentation

let HKSourceRevisionAnyVersion: String

A constant that matches any version.

let HKSourceRevisionAnyProductType: String

A constant that matches any product type.

let HKSourceRevisionAnyOperatingSystem: OperatingSystemVersion

A constant that matches any operating system.

### Creating Source Revision Objects

init(source: HKSource, version: String?)

Initializes a new source revision object with the provided source and version information.

