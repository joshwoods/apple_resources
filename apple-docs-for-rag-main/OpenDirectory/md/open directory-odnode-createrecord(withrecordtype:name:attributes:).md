

- Open Directory
- ODNode
-  createRecord(withRecordType:name:attributes:) 

Instance Method

# createRecord(withRecordType:name:attributes:)

Creates a record in a specified node with specified properties.

Mac CatalystmacOS 10.6+

``` source
func createRecord(
    withRecordType inRecordType: String!,
    name inRecordName: String!,
    attributes inAttributes: [AnyHashable : Any]! = [:]
) throws -> ODRecord
```

## Parameters 

`inRecordType`  

The record’s type.

`inRecordName`  

The record’s name.

`inAttributes`  

A dictionary of key-value pairs representing attributes for the record. Can be `nil`.

## Return Value

The created record.

## Discussion

The record is automatically assigned a UUID. This UUID can be overridden if one is specified in `inAttributes`.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Node Records

func record(withRecordType: String!, name: String!, attributes: Any!) throws -> ODRecord

Returns a record from the node with a specified type and name.

func supportedAttributes(forRecordType: String!) throws -> [Any]

Returns an array of attribute types supported by the node’s records.

func supportedRecordTypes() throws -> [Any]

Returns an array of the record types supported by the node.

