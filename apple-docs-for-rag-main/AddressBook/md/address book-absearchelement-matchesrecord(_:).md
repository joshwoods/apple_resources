

- Address Book
- ABSearchElement
-  matchesRecord(\_:) 

Instance Method

# matchesRecord(\_:)

Tests whether or not a record matches a search element.

macOS

``` source
func matchesRecord(_ record: ABRecord!) -> Bool
```

## Parameters 

`record`  

The record to be tested against the search object.

## Return Value

true if the `record` argument satisfies the conditions in the search element; otherwise, false.

## Discussion

If `record` is `nil`, this method raises an exception.

