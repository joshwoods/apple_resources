

- Contacts
- CNContactVCardSerialization
-  contacts(with:) 

Type Method

# contacts(with:)

Returns the contacts from the vCard data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func contacts(with data: Data) throws -> [CNContact]
```

## Parameters 

`data`  

The vCard data representing one or more contacts.

## Return Value

An array of contacts.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

