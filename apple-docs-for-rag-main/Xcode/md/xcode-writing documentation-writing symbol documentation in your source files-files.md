

- Xcode
- Writing documentation
-  Writing symbol documentation in your source files 

Article

# Writing symbol documentation in your source files

Add reference documentation to your symbols that explains how to use them.

## Overview

To help the people who use your API have a better understanding of it, follow the steps in the sections below to add documentation comments to the symbols in your project. DocC compiles those comments and generates formatted documentation that you share with your users. For frameworks and packages, add the comments to the public symbols, and for apps, add the comments to both the internal and public symbols.

For a deeper understanding of how to write symbol documentation, please refer to Writing Symbol Documentation in Your Source Files Swift.org.

### Add a basic description for each symbol

The first step toward writing great documentation is to add single-sentence abstracts or summaries, and where necessary, *Discussion* sections, to each of your public symbols.

Use the Code Actions menu in Xcode to generate a template that you fill out. Control-click the symbol in the source editor and choose Add Documentation from the Code Actions menu.

Replace the Description placeholder with a summary for the symbol.

Tip

The Add Documentation action recognizes the type of symbol and generates a template that includes placeholders for all the necessary elements, such as parameters and return values.

After you add a summary, Option-click the symbol to review the changes in Xcode’s Quick Help. It displays the text you add directly below the Summary header.

Any paragraphs you add appear below the Discussion header in Xcode’s Quick Help, and in the symbol reference page that DocC generates.

After adding a Discussion section, invoke Quick Help to view the updated documentation comment. Alternatively, choose Product \> Build Documentation to compile your documentation and open it in the documentation viewer.

### Describe the parameters of a method

For methods that take parameters, document those parameters directly below the summary, or the Discussion section, if you include one. Describe each parameter in isolation. Discuss its purpose and, where necessary, the range of acceptable values.

```
/// - Parameters:
///   - food: The food for the sloth to eat.
///   - quantity: The quantity of the food for the sloth to eat.
mutating public func eat(_ food: Food, quantity: Int) throws -> Int {
```

```
/// - Parameter food: The food for the sloth to eat.
/// - Parameter quantity: The quantity of the food for the sloth to eat.
mutating public func eat(_ food: Food, quantity: Int) throws -> Int {
```

After you add documentation for a method’s parameters, it appears in Xcode’s Quick Help, and in the symbol reference page that DocC generates when you choose Product \> Build Documentation.

### Describe the return value of a method

For methods that return a value, include a *Returns* section in your documentation comment to describe the returned value.

```
/// - Returns: The sloth's energy level after eating.
mutating public func eat(_ food: Food, quantity: Int) throws -> Int {
```

You can see your Returns section in the symbol reference page that DocC generates, as well as in Xcode’s Quick Help.

### Describe the thrown errors of a method

If a method can throw an error, add a *Throws* section to your documentation comment. Explain the circumstances that cause the method to throw an error, and list the types of possible errors.

```
/// - Throws: `SlothError.tooMuchFood` if the quantity is more than 100.
mutating public func eat(_ food: Food, quantity: Int) throws -> Int {
```

The Throws section appears in the symbol’s reference page, in the Quick Help pop-over, and in the Quick Help inspector that you can view using Command-Option-3.

## See Also

### Documentation content

Adding supplemental content to a documentation catalog

Include articles and extension files to extend your source documentation comments or provide supporting conceptual content.

SlothCreator: Building DocC Documentation in Xcode

Build DocC documentation for a Swift package that contains a DocC Catalog.

