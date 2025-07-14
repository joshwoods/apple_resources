

- Contacts
- CNContactStore
-  execute(\_:) 

Instance Method

# execute(\_:)

Executes a save request and returns success or failure.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func execute(_ saveRequest: CNSaveRequest) throws
```

## Parameters 

`saveRequest`  

The save request to execute.

## Return Value

true if the save request executes successfully; otherwise, false.

## Discussion

It is recommended that you do not access objects in the save request from other threads when it is in the process of being executed, because it may modify the contacts in the process. A save request only applies the changes to the objects. If there are overlapping changes with multiple or concurrent CNSaveRequest then the last saved change wins.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

