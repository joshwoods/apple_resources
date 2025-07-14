

- Address Book
- ABGroup
-  members() 

Instance Method

# members()

Returns an array of persons in a group.

macOS

``` source
func members() -> [Any]!
```

## Discussion

If this group doesn’t contain any people, this method returns an empty array.

## See Also

### Managing persons

func addMember(ABPerson!) -> Bool

Adds a person to a group.

func removeMember(ABPerson!) -> Bool

Removes a person from a group.

