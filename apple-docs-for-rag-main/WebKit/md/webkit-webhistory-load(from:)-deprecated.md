

- WebKit
- WebHistory
-  load(from:) Deprecated

Instance Method

# load(from:)

Loads the contents of the specified web history file.

macOS 10.3–10.14Deprecated

``` source
func load(from URL: URL!) throws
```

## Parameters 

`URL`  

The URL of the file to load. The file should have been created previously by a web history object. Note that the file’s format is private and should not be edited directly.

## Discussion

When successful, this method posts a notification (WebHistoryLoadedNotification).

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

class func setOptionalShared(WebHistory!)

Sets the web history object to share.

Deprecated

class func optionalShared() -> WebHistory!

Returns a shared web history object, if one exists.

Deprecated

### Loading and Saving History Information

func save(to: URL!) throws

Saves the web history to the specified file.

Deprecated

