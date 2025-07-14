

- Safari Services
- SSReadingList
-  addItem(with:title:previewText:) 

Instance Method

# addItem(with:title:previewText:)

Adds an item to the Reading List.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addItem(
    with URL: URL,
    title: String?,
    previewText: String?
) throws
```

## Parameters 

`URL`  

The URL of the item.

`title`  

The title of the item, or `nil`.

`previewText`  

A string shown as detail text for the item, or `nil`.

## Discussion

Call this method when the user chooses to add to the Reading List.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

