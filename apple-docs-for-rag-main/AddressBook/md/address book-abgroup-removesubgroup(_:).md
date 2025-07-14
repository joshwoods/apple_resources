

- Address Book
- ABGroup
-  removeSubgroup(\_:) 

Instance Method

# removeSubgroup(\_:)

Removes a subgroup from a group.

macOS

``` source
func removeSubgroup(_ group: ABGroup!) -> Bool
```

## Parameters 

`group`  

The subgroup to be removed.

## Return Value

true if successful; otherwise, false.

## Discussion

If the `group` argument is not a subgroup, this method does nothing and returns false. If `group` is `nil`, this method raises an exception.

## See Also

### Managing subgroups

func addSubgroup(ABGroup!) -> Bool

Adds a subgroup to another group.

func parentGroups() -> [Any]!

Returns an array containing a group’s parents—that is, the groups that a group belongs to.

func subgroups() -> [Any]!

Returns an array containing a group’s subgroups.

