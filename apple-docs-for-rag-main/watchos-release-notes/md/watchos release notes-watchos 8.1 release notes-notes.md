

- watchOS Release Notes
-  watchOS 8.1 Release Notes 

Article

# watchOS 8.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 8 SDK provides support to develop watchOS apps for Apple Watch devices running watchOS 8.1. The SDK comes bundled with Xcode 13, available from the Mac App Store. For information on the compatibility requirements for Xcode 13, see Xcode 13 Release Notes.

### CoreData

#### Known Issues

- `NSExpression` immediately forbids certain operations that have significant side effects, like creating and destroying objects. Additionally, casting string class names into Class objects with `NSConstantValueExpression` is deprecated. (84017178)

  **Workaround:** Pass temporary objects to `NSExpression` in the context parameter of expressionValueWithObject:context:, or with `NSPredicate` as the `substitutionVariables` parameter of evaluateWithObject:substitutionVariables:. You can create a derived predicate with all the substitution variables replaced (bound), using withSubstitutionVariables(_:) on an existing `NSPredicate` so that code using the object can continue to use a simple `evaluate(with object: Any?)` invocation.

## See Also

### watchOS 8

watchOS 8.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 8.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 8.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 8.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 8.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 8 Release Notes

Update your apps to use new features, and test your apps against API changes.

