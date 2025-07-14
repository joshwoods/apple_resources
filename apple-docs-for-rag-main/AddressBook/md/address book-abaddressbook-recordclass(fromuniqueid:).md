

- Address Book
- ABAddressBook
-  recordClass(fromUniqueId:) 

Instance Method

# recordClass(fromUniqueId:)

Returns the class name of the record that matches the given unique ID.

macOS 10.3+

``` source
func recordClass(fromUniqueId uniqueId: String!) -> String!
```

## Parameters 

`uniqueId`  

The unique ID of the record.

## Return Value

The name of the class of the record, for example `ABPerson`.

