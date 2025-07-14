

- Open Directory
- ODRecord
-  isMemberRecord(\_:) 

Instance Method

# isMemberRecord(\_:)

Determines whether a given record is a member of this group record.

Mac CatalystmacOS 10.6+

``` source
func isMemberRecord(_ inRecord: ODRecord!) throws
```

## Parameters 

`inRecord`  

The record to test for membership.

## Discussion

If this record is not a group record, this method returns false.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Group Records

func addMemberRecord(ODRecord!) throws

Adds a member record to this group record.

func removeMemberRecord(ODRecord!) throws

Removes a record as a member of this group record.

