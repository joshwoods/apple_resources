

- XcodeKit
- XCSourceEditorCommand
-  perform(with:completionHandler:) 

Instance Method

# perform(with:completionHandler:)

Performs the action associated with the command using the information in an invocation.

macOS 10.12+

``` source
func perform(
    with invocation: XCSourceEditorCommandInvocation,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func perform(with invocation: XCSourceEditorCommandInvocation) async throws
```

**Required**

## Parameters 

`invocation`  

The invocation of the command to be invoked.

`completionHandler`  

A block to be executed when the command finishes.

## Mentioned in 

Creating a Source Editor Extension

Testing Your Source Editor Extension

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func perform(with invocation: XCSourceEditorCommandInvocation) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Xcode passes the code a completion handler that it must invoke to finish performing the command, passing `nil` on success or an error on failure. A canceled command must still call the completion handler, passing `nil`.

There are no guarantees about the thread or queue on which the cancellation handler is invoked.

