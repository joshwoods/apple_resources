

- Address Book
- ABAddressBook
-  records(matching:) 

Instance Method

# records(matching:)

Returns an array of records that match the given search element, or returns an empty array if no records match the search element.

macOS

``` source
func records(matching search: ABSearchElement!) -> [Any]!
```

## Parameters 

`search`  

The search element to perform the search against.

## Return Value

An array of records that match the given search element, or an empty array if no records match the search element.

## Discussion

If `search` is `nil`, this method raises an exception.

