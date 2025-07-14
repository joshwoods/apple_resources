

- Core WLAN
- CWInterface
-  commitConfiguration(\_:authorization:) 

Instance Method

# commitConfiguration(\_:authorization:)

Commit a configuration for the given WLAN interface.

macOS 10.7+

``` source
func commitConfiguration(
    _ configuration: CWConfiguration,
    authorization: SFAuthorization?
) throws
```

## Parameters 

`configuration`  

The configuration to commit.

`authorization`  

An SFAuthorization object to use for authorizing the commit. This parameter is optional and can be passed as *nil*.

## Discussion

This method requires the caller have root privileges or obtain administrator privileges with the *authorization* parameter.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

