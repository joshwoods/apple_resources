

- Core Data
-  NSFetchRequestExpression 

Class

# NSFetchRequestExpression

An expression that evaluates the result of a fetch request on a managed object context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSFetchRequestExpression
```

## Overview

`NSFetchRequestExpression` inherits from NSExpression, which provides most of the basic behavior. The first argument must be an expression which evaluates to an `NSFetchRequest` object, and the second must be an expression which evaluates to an `NSManagedObjectContext` object. If you simply want the count for the request, the `countOnly` argument should be true.

## Topics

### Creating a Fetch Request Expression

class func expression(forFetch: NSExpression, context: NSExpression, countOnly: Bool) -> NSExpression

Returns an expression which will evaluate to the result of executing a fetch request on a context.

### Examining a Fetch Request Expression

var requestExpression: NSExpression

The expression for the receiver’s fetch request.

var contextExpression: NSExpression

The expression for the receiver’s managed object context.

var isCountOnlyRequest: Bool

Returns a Boolean value that indicates whether the receiver represents a count-only fetch request.

### Constants

let NSFetchRequestExpressionType: NSExpression.ExpressionType

This constant specifies the fetch request expression type.

## Relationships

### Inherits From

- NSExpression

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

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

class NSExpressionDescription

An object that describes an expression to include with a fetch request.

class NSFetchedPropertyDescription

A description object used to define which properties are fetched from Core Data.

