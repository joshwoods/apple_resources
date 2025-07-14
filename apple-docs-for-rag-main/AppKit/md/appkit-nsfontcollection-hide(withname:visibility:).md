

- AppKit
- NSFontCollection
-  hide(withName:visibility:) 

Type Method

# hide(withName:visibility:)

Remove from view the named font collection with the specified visibility.

macOS 10.7+

``` source
class func hide(
    withName name: NSFontCollection.Name,
    visibility: NSFontCollection.Visibility
) throws
```

## Parameters 

`name`  

The name of the collection.

`visibility`  

The visibility of the collection.

## Discussion

For a persistent font collection, this method deletes the named font collection from disk.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Naming the Font Collection

class func rename(fromName: NSFontCollection.Name, visibility: NSFontCollection.Visibility, toName: NSFontCollection.Name) throws

Renames the font collection with the specified name and visibility to the second name specified.

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class var allFontCollectionNames: [NSFontCollection.Name]

Returns all named collections visible to this process.

struct Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

struct Visibility

Constants that specify the visibility of font collections.

