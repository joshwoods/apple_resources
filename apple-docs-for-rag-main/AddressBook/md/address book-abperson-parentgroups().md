

- Address Book
- ABPerson
-  parentGroups() 

Instance Method

# parentGroups()

Returns an array of the address book groups that this person belongs to.

macOS

``` source
func parentGroups() -> [Any]!
```

## Discussion

If the person doesn’t belong to any groups, this method returns an empty array.

