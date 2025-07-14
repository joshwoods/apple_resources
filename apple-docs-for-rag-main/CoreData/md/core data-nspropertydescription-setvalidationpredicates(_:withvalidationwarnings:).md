

- Core Data
- NSPropertyDescription
-  setValidationPredicates(\_:withValidationWarnings:) 

Instance Method

# setValidationPredicates(\_:withValidationWarnings:)

Sets the validation predicates and warnings of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setValidationPredicates(
    _ validationPredicates: [NSPredicate]?,
    withValidationWarnings validationWarnings: [String]?
)
```

## Parameters 

`validationPredicates`  

An array containing the validation predicates for the receiver.

`validationWarnings`  

An array containing the validation warnings for the receiver.

## Discussion

The `validationPredicates` and `validationWarnings` arrays should contain the same number of elements, and corresponding elements should appear at the same index in each array.

Instead of implementing individual validation methods, you can use this method to provide a list of predicates that are evaluated against the managed objects and a list of corresponding error messages (which can be localized).

### Special Considerations

This method raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Supporting Validation

var validationPredicates: [NSPredicate]

The validation predicates of the receiver.

var validationWarnings: [Any]

The error strings associated with the receiver’s validation predicates.

