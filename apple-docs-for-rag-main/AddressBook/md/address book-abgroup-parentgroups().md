

- Address Book
- ABGroup
-  parentGroups() 

Instance Method

# parentGroups()

Returns an array containing a group’s parents—that is, the groups that a group belongs to.

macOS

``` source
func parentGroups() -> [Any]!
```

## Discussion

If this group doesn’t belong to any groups, this method returns an empty array.

## See Also

### Managing subgroups

func addSubgroup(ABGroup!) -> Bool

Adds a subgroup to another group.

func removeSubgroup(ABGroup!) -> Bool

Removes a subgroup from a group.

func subgroups() -> [Any]!

Returns an array containing a group’s subgroups.

