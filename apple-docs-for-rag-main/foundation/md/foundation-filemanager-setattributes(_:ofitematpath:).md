

- Foundation
- FileManager
-  setAttributes(\_:ofItemAtPath:) 

Instance Method

# setAttributes(\_:ofItemAtPath:)

Sets the attributes of the specified file or directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setAttributes(
    _ attributes: [FileAttributeKey : Any],
    ofItemAtPath path: String
) throws
```

## Parameters 

`attributes`  

A dictionary containing as keys the attributes to set for `path` and as values the corresponding value for the attribute. You can set the following attributes: busy, creationDate, extensionHidden, groupOwnerAccountID, groupOwnerAccountName, hfsCreatorCode, hfsTypeCode, immutable, modificationDate, ownerAccountID, ownerAccountName, posixPermissions. You can change single attributes or any combination of attributes; you need not specify keys for all attributes.

`path`  

The path of a file or directory.

## Discussion

As in the POSIX standard, the app either must own the file or directory or must be running as superuser for attribute changes to take effect. The method attempts to make all changes specified in attributes and ignores any rejection of an attempted modification. If the last component of the path is a symbolic link, the system traverses it.

You must initialize the posixPermissions value with the code representing the POSIX file-permissions bit pattern. The system sets hfsCreatorCode and hfsTypeCode only when `path` specifies a file.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Getting and Setting Attributes

func componentsToDisplay(forPath: String) -> [String]?

Returns an array of strings representing the user-visible components of a given path.

func displayName(atPath: String) -> String

Returns the display name of the file or directory at a specified path.

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func attributesOfFileSystem(forPath: String) throws -> [FileAttributeKey : Any]

Returns a dictionary that describes the attributes of the mounted file system on which a given path resides.

