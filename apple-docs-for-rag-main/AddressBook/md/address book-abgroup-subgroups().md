

- Address Book
- ABGroup
-  subgroups() 

Instance Method

# subgroups()

Returns an array containing a group’s subgroups.

macOS

``` source
func subgroups() -> [Any]!
```

## Discussion

If this group doesn’t contain any groups, this method returns an empty array.

## See Also

### Managing subgroups

func addSubgroup(ABGroup!) -> Bool

Adds a subgroup to another group.

func removeSubgroup(ABGroup!) -> Bool

Removes a subgroup from a group.

func parentGroups() -> [Any]!

Returns an array containing a group’s parents—that is, the groups that a group belongs to.

