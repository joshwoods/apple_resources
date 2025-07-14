

- Swift Playgrounds
- Playground Books
-  Creating and Running a Playground Book 

Article

# Creating and Running a Playground Book

Build a playground book from a template, and run it in Swift Playgrounds.

## Overview

You use both a Mac running Xcode and an iPad to create a playground book. You download the Swift Playgrounds Author Template and open it in Xcode on a Mac. You then write pages for the book and package its resources into a `.playgroundbook` file that you share with an iPad.

Important

The Swift Playgrounds Author Template is deprecated and may not be compatible with future versions of Xcode. You can continue working with Playground Books by editing their contents directly in Xcode and other tools. In Finder, select and control-click on your Playground Book, and choose “Show Package Contents”. For details on working with the structure and format, see Playground Books. For information on working with the Swift Playgrounds App and Swift Package formats, see Swift Playgrounds and Swift.org.”

### Extract and Open the Template

The Swift Playgrounds Author Template is packaged as a `.xip` archive. To open the template, navigate to it in Finder and double-click it to extract it into a folder called Swift_Playgrounds_Author_Template_for_Xcode. Navigate within that folder to the Template subfolder and open the Xcode project named PlaygroundBook.

### Build the Playground Book

The template contains all the initial files and resources you need to start writing content for Swift Playgrounds. Choose `Product > Build` to compile these resources into a `.playgroundbook` file that you can share with an iPad.

### Run the Playground Book on Your iPad

To run the built playground book, transfer it to Swift Playgrounds:

1.  Open Finder and select AirDrop.

2.  In the project navigator for the template in Xcode, open the Products folder.

3.  Drag the `.playgroundbook` file over Finder and drop it on the icon representing your iPad.

Swift Playgrounds automatically opens when you share a playground book.

The following image shows the content from the template running in Swift Playgrounds.

## See Also

### Playground Setup

Structuring Content for Swift Playgrounds

Add content to a playground book by creating new folders and property lists.

