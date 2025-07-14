

- WebKit
- WebHistory
-  save(to:) Deprecated

Instance Method

# save(to:)

Saves the web history to the specified file.

macOS 10.3–10.14Deprecated

``` source
func save(to URL: URL!) throws
```

## Parameters 

`URL`  

The URL of the file to contain the web history information. The file must be user-writable, but its format is private and should not be edited directly.

## Discussion

When successful, this method posts a notification (WebHistorySavedNotification).

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Loading and Saving History Information

func load(from: URL!) throws

Loads the contents of the specified web history file.

Deprecated

