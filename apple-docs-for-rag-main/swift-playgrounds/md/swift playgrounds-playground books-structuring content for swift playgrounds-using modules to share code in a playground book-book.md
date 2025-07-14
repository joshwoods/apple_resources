

- Swift Playgrounds
- Playground Books
- Structuring Content for Swift Playgrounds
-  Using Modules to Share Code in a Playground Book 

Article

# Using Modules to Share Code in a Playground Book

In Swift Playgrounds 3.0 and later, make code available across multiple chapters to teach the value of reusable code.

## Overview

Where you place the code in a book determines its visibilty to other parts of the book. For example, the code in the `main.swift` file on a page isn’t visible to the rest of the book. If your book contains multiple pages or chapters that require access to a shared codebase, place the code in a module. The following screenshot shows files from multiple modules open across several tabs:

By sharing code throughout your book, you provide consistent APIs that teach a common interface.

### Share Code with Modules

Modules are folders of Swift code that you use to define APIs for learners to use, while also implementing functionality for your pages’ live views. There are two kinds of modules:

- Private Modules: Code that learners don’t need to inspect or edit. Public APIs and documentation you define in these modules, however, are still available to learners. Place these modules in the `.playgroundbook/Contents/Modules` directory.

- User-Editable Modules: Use when the code is part of the instructive content of your book. For example, you might teach the value of code reuse by having learners leverage their code from previous chapters in the solution to a problem in a subsequent chapter. Place these modules in the `.playgroundbook/Contents/UserModules` directory.

Place each module in the Modules or UserModules directory in a new directory that ends with the suffix `.playgroundmodule`. Place module source code in a directory named Sources within the `.playgroundmodule` directory. For example, to define a user-editable module named Statistics, place code in a path such as `UserModules/Statistics.playgroundmodule/Sources/MyStatisticsAPIs.swift`.

Module names must be valid Swift identifiers, so the `.playgroundmodule` directory name can’t include invalid character sequences, like spaces.

Important

If you’re writing a book that targets a version of the Swift Playgrounds book format earlier than 6.0, modules are unavailable. Instead, add code in a directory named Sources that’s adjacent to the PublicResources or PrivateResources directory in a book, chapter, or page.

## See Also

### Book Structure

Adding a Chapter to a Playground Book

Create a folder with a manifest that describes the chapter’s name and page order.

Adding a Page to a Playground Book

Create a subfolder, a manifest file, and a content file.

Adding a Cutscene to a Playground Book

Create a subfolder, a manifest file, and cutscene metadata.

Sharing Resources in a Playground Book

Reuse common assets throughout a book to reduce its size.

