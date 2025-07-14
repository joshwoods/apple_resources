

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:validate:) 

Instance Method

# panel(\_:validate:)

Asks the delegate to validate the URL for a file that the user selected.

macOS 10.6+

``` source
@MainActor
optional func panel(
    _ sender: Any,
    validate url: URL
) throws
```

## Parameters 

`sender`  

The panel that requests URL validation.

`url`  

The URL for you to validate.

## Discussion

Save panels call this method when the user clicks the Save button. Open panels call it when the user clicks the Open button. An Open panel calls this method once for each selected filename or directory.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Validating the Panel Content

func panel(Any, shouldEnable: URL) -> Bool

Asks the delegate whether the specified URL should be enabled in the Open panel.

