

- Open Directory
- ODNode
-  record(withRecordType:name:attributes:) 

Instance Method

# record(withRecordType:name:attributes:)

Returns a record from the node with a specified type and name.

Mac CatalystmacOS 10.6+

``` source
func record(
    withRecordType inRecordType: String!,
    name inRecordName: String!,
    attributes inAttributes: Any!
) throws -> ODRecord
```

## Parameters 

`inRecordType`  

The type of the record.

`inRecordName`  

The name of the record.

`inAttributes`  

An array of record attributes to be cached before the record is returned. Can be `nil`.

## Return Value

The requested record.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Node Records

func createRecord(withRecordType: String!, name: String!, attributes: [AnyHashable : Any]!) throws -> ODRecord

Creates a record in a specified node with specified properties.

func supportedAttributes(forRecordType: String!) throws -> [Any]

Returns an array of attribute types supported by the node’s records.

func supportedRecordTypes() throws -> [Any]

Returns an array of the record types supported by the node.

