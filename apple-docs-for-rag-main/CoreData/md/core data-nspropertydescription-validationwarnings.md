

- Core Data
- NSPropertyDescription
-  validationWarnings 

Instance Property

# validationWarnings

The error strings associated with the receiver’s validation predicates.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var validationWarnings: [Any] { get }
```

## See Also

### Supporting Validation

var validationPredicates: [NSPredicate]

The validation predicates of the receiver.

func setValidationPredicates([NSPredicate]?, withValidationWarnings: [String]?)

Sets the validation predicates and warnings of the receiver.

