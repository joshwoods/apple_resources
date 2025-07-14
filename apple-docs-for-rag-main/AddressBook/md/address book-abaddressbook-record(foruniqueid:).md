

- Address Book
- ABAddressBook
-  record(forUniqueId:) 

Instance Method

# record(forUniqueId:)

Returns the person or group record that matches the given unique ID.

macOS

``` source
func record(forUniqueId uniqueId: String!) -> ABRecord!
```

## Parameters 

`uniqueId`  

The unique ID of the record. This value must not be `nil`; otherwise, an exception is raised.

## Return Value

The person or group record that matches the given unique ID.

## Discussion

If no record has the given ID, this method returns `nil`.

