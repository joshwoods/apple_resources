

- Address Book
- ABGroup
-  addSubgroup(\_:) 

Instance Method

# addSubgroup(\_:)

Adds a subgroup to another group.

macOS

``` source
func addSubgroup(_ group: ABGroup!) -> Bool
```

## Parameters 

`group`  

The group to add as a subgroup.

## Return Value

true if successful; otherwise, false.

## Discussion

If the `group` argument is already part of the receiver, this method does nothing and returns false. If adding the group would create a recursion, this method also does nothing and returns false. (For example, if the group Animal Lovers is in Dog Lovers, and you add Dog Lovers to Animal Lovers, that would create a recursion, which this method won’t allow.) If the `group` argument is `nil`, this method raises an exception.

## See Also

### Managing subgroups

func removeSubgroup(ABGroup!) -> Bool

Removes a subgroup from a group.

func parentGroups() -> [Any]!

Returns an array containing a group’s parents—that is, the groups that a group belongs to.

func subgroups() -> [Any]!

Returns an array containing a group’s subgroups.

