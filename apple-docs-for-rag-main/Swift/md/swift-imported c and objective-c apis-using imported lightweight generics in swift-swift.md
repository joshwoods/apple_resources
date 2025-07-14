

- Swift
- Imported C and Objective-C APIs
-  Using Imported Lightweight Generics in Swift 

Article

# Using Imported Lightweight Generics in Swift

Understand the constraints of imported Obj-C lightweight generic type declarations.

## Overview

Objective-C type declarations that use lightweight generic parameterization are imported by Swift with information about the type of their contents preserved. For example, given the following Objective-C property declarations:

```
@property NSArray *dates;
@property NSCache> *cachedData;
@property NSDictionary  *> *supportedLocales;
```

Here’s the Swift version of those declarations when you import them:

```
var dates: [Date]
var cachedData: NSCache
var supportedLocales: [String: [Locale]]
```

A parameterized class written in Objective-C is imported into Swift as a generic class with the same number of type parameters. All Objective-C generic type parameters imported by Swift have a type constraint that requires that type to be a class (`T: AnyObject`).

If the Objective-C generic parameterization specifies class or protocols qualifications, the imported Swift declaration has a constraint that requires that type to be a subclass of the specified class or to conform to the specified protocol. For an unspecialized Objective-C type, Swift infers the generic parameterization for the imported class type constraints. For example, consider the following Objective-C class and category declarations:

```
@interface List> : NSObject
- (List *)listByAppendingItemsInList:(List *)otherList;
@end

@interface ListContainer : NSObject
- (List *)listOfValues;
@end

@interface ListContainer (ObjectList)
- (List *)listOfObjects;
@end
```

When you import these declarations into Swift, the `NSCopying` protocol qualification of the `List` type and the `NSValue` class qualification of the `listOfValues` method are preserved. In addition, the unqualified `listOfObjects` method uses the `NSCopying` generic constraint inferred from the `List` type.

```
class List : NSObject {
    func listByAppendingItemsInList(otherList: List) -> List
}

class ListContainer : NSObject {
    func listOfValues() -> List
}

extension ListContainer {
    func listOfObjects() -> List
}
```

## See Also

### Objective-C APIs

Using Imported Protocol-Qualified Classes in Swift

Learn how imported Objective-C protocol-qualified classes and metaclasses are represented.

