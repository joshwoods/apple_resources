

- Swift Playgrounds
- Playground Books
- Structuring Content for Swift Playgrounds
-  Adding a Chapter to a Playground Book 

Article

# Adding a Chapter to a Playground Book

Create a folder with a manifest that describes the chapter’s name and page order.

## Overview

You use chapters to group the pages of a playground book by topic.

### Create a Chapter Folder

Create a new folder in the Chapters folder inside your playground book’s Contents folder. The new chapter’s folder name must end with the suffix .playgroundchapter.

In Xcode, create a property list file called `Manifest.plist` in the new chapter’s folder. Choose File \> New \> File, then choose the Property List template from iOS \> Resources. Use the manifest property list to list the chapter’s name and the order of its pages, which can include both playground pages (.playgroundpage) and cutscene pages (.cutscenepage).

The following image shows the example chapter, “First Chapter,” which contains two pages.

### Name the Chapter

Choose a name for your new chapter by adding a `Name` key to the `Manifest.plist` property list. This name is displayed to learners in the table of contents for your book in Swift Playgrounds.

### Arrange Pages in the Chapter

Pages in your playground book must be placed in a chapter. The page folders you place within chapter folders determine which pages go into which chapters. You choose the *order* of pages in a chapter by adding a `Pages` key to the chapter’s `Manifest.plist` file. The `Pages` key is an ordered array of page folder names. Add the names of a chapter’s pages in the order in which you want those pages to appear in the chapter.

## See Also

### Book Structure

Adding a Page to a Playground Book

Create a subfolder, a manifest file, and a content file.

Adding a Cutscene to a Playground Book

Create a subfolder, a manifest file, and cutscene metadata.

Using Modules to Share Code in a Playground Book

In Swift Playgrounds 3.0 and later, make code available across multiple chapters to teach the value of reusable code.

Sharing Resources in a Playground Book

Reuse common assets throughout a book to reduce its size.

