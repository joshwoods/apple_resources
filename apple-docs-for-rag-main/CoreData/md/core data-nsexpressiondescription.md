

- Core Data
-  NSExpressionDescription 

Class

# NSExpressionDescription

An object that describes an expression to include with a fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSExpressionDescription
```

## Overview

An expression description describes a value that a fetch request returns, which doesn’t appear as an attribute or relationship on an entity. For example, expressions can aggregate data, or transform an attribute’s value. You add expression descriptions to a fetch request using the propertiesToFetch method.

Important

Don’t add expression descriptions to the properties array of NSEntityDescription.

## Topics

### Configuring the Expression Description

var expression: NSExpression?

The expression to evaluate.

var resultType: NSAttributeDescription.AttributeType

The attribute type of the expression’s result.

var expressionResultType: NSAttributeType

The attribute type of the expression’s result.

Deprecated

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSPropertyDescription

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Specifying Fetch Constraints

var predicate: NSPredicate?

The predicate of the fetch request.

var fetchLimit: Int

The fetch limit of the fetch request.

var fetchOffset: Int

The fetch offset of the fetch request.

var fetchBatchSize: Int

The batch size of the objects specified in the fetch request.

var affectedStores: [NSPersistentStore]?

An array of persistent stores specified for the fetch request.

class NSFetchRequestExpression

An expression that evaluates the result of a fetch request on a managed object context.

class NSFetchedPropertyDescription

A description object used to define which properties are fetched from Core Data.

