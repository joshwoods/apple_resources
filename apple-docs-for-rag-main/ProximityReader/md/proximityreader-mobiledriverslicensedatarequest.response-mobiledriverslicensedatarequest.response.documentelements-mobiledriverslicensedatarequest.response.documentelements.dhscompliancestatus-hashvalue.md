

- ProximityReader
- MobileDriversLicenseDataRequest
- 
  - MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
- MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

