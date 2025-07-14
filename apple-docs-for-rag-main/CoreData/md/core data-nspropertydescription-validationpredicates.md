

- Core Data
- NSPropertyDescription
-  validationPredicates 

Instance Property

# validationPredicates

The validation predicates of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var validationPredicates: [NSPredicate] { get }
```

## See Also

### Supporting Validation

var validationWarnings: [Any]

The error strings associated with the receiver’s validation predicates.

func setValidationPredicates([NSPredicate]?, withValidationWarnings: [String]?)

Sets the validation predicates and warnings of the receiver.

