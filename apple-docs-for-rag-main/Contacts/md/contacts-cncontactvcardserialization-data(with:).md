

- Contacts
- CNContactVCardSerialization
-  data(with:) 

Type Method

# data(with:)

Returns the vCard representation of the specified contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func data(with contacts: [CNContact]) throws -> Data
```

## Parameters 

`contacts`  

An array of contacts.

## Return Value

An NSData object with the vCard representation of the contact.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

