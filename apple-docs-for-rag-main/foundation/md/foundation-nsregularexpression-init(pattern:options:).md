

- Foundation
- NSRegularExpression
-  init(pattern:options:) 

Initializer

# init(pattern:options:)

Returns an initialized NSRegularExpression instance with the specified regular expression pattern and options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    pattern: String,
    options: NSRegularExpression.Options = []
) throws
```

## Parameters 

`pattern`  

The regular expression pattern to compile.

`options`  

The regular expression options that are applied to the expression during matching. See NSRegularExpression.Options for possible values.

## Return Value

An instance of `NSRegularExpression` for the specified regular expression and options.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

