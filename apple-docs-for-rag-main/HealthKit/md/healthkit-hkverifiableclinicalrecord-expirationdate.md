

- HealthKit
- HKVerifiableClinicalRecord
-  expirationDate 

Instance Property

# expirationDate

The date when the card expires.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
var expirationDate: Date? { get }
```

## See Also

### Reading Metadata

var issuedDate: Date

The date when the issuer created the card.

var relevantDate: Date

A date relevant to this record, such as when the issuer administered a vaccine or performed a test.

var recordTypes: [String]

An array of strings representing the types of records contained in the card.

var sourceType: HKVerifiableClinicalRecordSourceType?

The source for the verifiable clinical record

struct HKVerifiableClinicalRecordSourceType

The source type for the verifiable clinical record.

var itemNames: [String]

A human-readable description of the card’s contents.

