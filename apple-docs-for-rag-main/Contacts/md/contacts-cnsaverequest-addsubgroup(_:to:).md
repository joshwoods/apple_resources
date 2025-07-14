

- Contacts
- CNSaveRequest
-  addSubgroup(\_:to:) 

Instance Method

# addSubgroup(\_:to:)

Add the specified group to a parent group.

macOS 10.11+

``` source
func addSubgroup(
    _ subgroup: CNGroup,
    to group: CNGroup
)
```

## Parameters 

`subgroup`  

The subgroup to add.

`group`  

The parent group in which to add `subgroup`.

## Discussion

If you previously tried to remove `subgroup` from `group` in the same save request, calling this method undoes that removal. The last change you make is the one that takes effect.

## See Also

### Adding and removing subgroups

func removeSubgroup(CNGroup, from: CNGroup)

Remove a subgroup from the specified parent group.

