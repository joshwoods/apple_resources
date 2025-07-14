

- Foundation
- NSUserScriptTask
-  init(url:) 

Initializer

# init(url:)

Return a user script task instance given a URL for a script file.

macOS 10.8+

``` source
init(url: URL) throws
```

## Parameters 

`url`  

The script URL.

## Return Value

An instance of an `NSUserScriptTask` subclass or `nil` if the file does not appear to match any of the known types.

## Discussion

The returned object will be of one of the specific sub-classes (NSUserUnixTask, NSUserAppleScriptTask, and NSUserAutomatorTask), or `nil` if the file does not appear to match any of the known types.

If invoked from a subclass, the result will be that class or `nil`.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Specifying the Script

var scriptURL: URL

The URL of the script file.

