

- HealthKit
- HKFHIRVersion
-  init(fromVersionString:) 

Initializer

# init(fromVersionString:)

Creates an FHIR version object from a string representation of the version.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+

``` source
convenience init(fromVersionString versionString: String) throws
```

## Parameters 

`versionString`  

A string representing the version.

## Discussion

The string must be in the following format: `..`.

## See Also

### Creating Version Objects

class func primaryDSTU2() -> Self

Returns the primary Second Draft Standard for Trial Use (DSTU2) version.

class func primaryR4() -> Self

Returns the primary Release 4 (R4) version.

