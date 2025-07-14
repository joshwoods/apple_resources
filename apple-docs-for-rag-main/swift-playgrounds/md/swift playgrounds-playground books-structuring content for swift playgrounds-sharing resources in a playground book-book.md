

- Swift Playgrounds
- Playground Books
- Structuring Content for Swift Playgrounds
-  Sharing Resources in a Playground Book 

Article

# Sharing Resources in a Playground Book

Reuse common assets throughout a book to reduce its size.

## Overview

Where you place an asset in a book determines its visibility to other parts of the book. If multiple pages or chapters require access to a shared resource, place those resources closer to the root of your book’s directory structure. For example, the images in a page’s PublicResources directory aren’t visible to the rest of the book.

### Share Resources

How you share a resource depends largely on where you intend to use that resource:

- When sharing on a single page or cutscene, place the resources in the PublicResources or PrivateResources directory of the `.playgroundpage` directory or `.cutscenepage` directory.

- When sharing a resource among the pages of a chapter, place the resources in the PublicResources or PrivateResources directory of the `.playgroundchapter` directory.

- When sharing resources throughout an entire book, place the resources in the PublicResources or PrivateResources directory of the book’s Contents directory.

Public resources are visible to and usable by learners. For example, if you want learners to select one of several images in their code, place the resource in the PublicResources directory; otherwise, place it in the PrivateResources directory.

### Share Localized Resources

If you support multiple localizations of content in your book, share localized resources by placing them in localization project directories within either the PublicResources or PrivateResources directory. Name localization project directories according to the language ID of the localization, followed by the `.lproj` suffix. For example, a book localized to English and French might have shared chapter resources in two locations:

- `mybook.playgroundbook/Contents/Chapters/ch1.playgroundchapter/PublicResources/en.lproj` for the English localization.

- `mybook.playgroundbook/Contents/Chapters/ch1.playgroundchapter/PublicResources/fr.lproj` for the French localization.

To determine which identifier to use for a particular localization, see Language IDs.

## See Also

### Book Structure

Adding a Chapter to a Playground Book

Create a folder with a manifest that describes the chapter’s name and page order.

Adding a Page to a Playground Book

Create a subfolder, a manifest file, and a content file.

Adding a Cutscene to a Playground Book

Create a subfolder, a manifest file, and cutscene metadata.

Using Modules to Share Code in a Playground Book

In Swift Playgrounds 3.0 and later, make code available across multiple chapters to teach the value of reusable code.

