

- Xcode
- Writing documentation
-  Adding supplemental content to a documentation catalog 

Article

# Adding supplemental content to a documentation catalog

Include articles and extension files to extend your source documentation comments or provide supporting conceptual content.

## Overview

The process of crafting great documentation is an art. Your content is unique; you know which elements, beyond source documentation comments, provide the most value to your readers. For information about adding supplemental content to a documentation catalog with DocC, see Adding Supplemental Content to a Documentation Catalog Swift.Org.

### Add articles to explain concepts or describe tasks

If your documentation catalog includes an article file with the name `GettingStarted.md`, Xcode displays this article in the documentation viewer with a document icon.

The structure of an article is similar to symbol files or a top-level landing page, with the exception that the first level 1 header is regular content instead of a symbol reference. For example, the Getting Started with Sloths article contains the following title, single-sentence abstract or summary, and Overview section:

```
# Getting started with sloths

Create a sloth and assign personality traits and abilities.

## Overview

Sloths are complex creatures that require careful creation and a suitable
habitat.
...
```

After the Overview section, additional sections and subsections use a double hash (##) for a level 2 header, and a triple hash (###) for a level 3 header. Follow the hashes with a space, and then the title for that section or subsection.

To add an article to your documentation catalog in Xcode, do the following:

1.  Select your documentation catalog in the Project navigator.

2.  Choose File \> New \> File to open the file template chooser.

3.  Select the Article File template in the Documentation section and click Next.

4.  Enter a filename and click Create. Xcode creates a new article file with a default name.

5.  Modify the first line of the file to specify its title.

6.  Replace the summary and placeholders in the file with appropriate content.

### Add extension files to append to or override source documentation comments

DocC supports supplementing or completely replacing source documentation comments with content in extension files. To add an extension file to your documentation catalog, do the following:

1.  In Xcode, select your documentation catalog in the Project navigator.

2.  Choose File \> New \> File to open the file template chooser.

3.  Select the Extension File template in the Documentation section and click Next.

4.  Enter the symbol name as the filename and click Create.

5.  Modify the first line of the file to identify the symbol that the file relates to.

In the extension file, replace the `Symbol` placeholder with the absolute path to the symbol. The absolute path is the target’s product module name followed by the symbol name.

## See Also

### Documentation content

Writing symbol documentation in your source files

Add reference documentation to your symbols that explains how to use them.

SlothCreator: Building DocC Documentation in Xcode

Build DocC documentation for a Swift package that contains a DocC Catalog.

