

- Swift Playgrounds
- Playground Books
-  Writing Prose for a Playground Page 

Article

# Writing Prose for a Playground Page

Add comment markers in your Swift code to mark text as prose.

## Overview

Playground pages almost always need prose to introduce the concepts you’re teaching on the page. You use a special kind of Swift comment to mark single lines or blocks of text as prose. When a playground page’s `main.swift` file is displayed in Swift Playgrounds, comments marked as prose are displayed using a proportional font.

### Add Single-Line Prose

To add short sections of prose to a page, write a single-line Swift comment that starts with a colon (`//:`).

```
//: This line contains a short sentence.
```

Comments without the colon are treated as normal Swift comments and are displayed in a monospace font. Text that’s outside of any sort of comment is treated as Swift code and runs when you tap Run My Code.

You can use markup in prose to add semantic treatments like emphasis and code voice. For information on supported markup, see Markup Formatting Reference.

### Add Multiline Prose

Use multiline Swift comments for longer passages. You indicate that a multiline comment is prose by adding a colon immediately after the comment’s starting delimiter (`/*:`).

```
/*:
    Roses are `UIColor.red`,
    Violets are 🔵,
    Swift Playgrounds are rad,
    and so are you!
*/
```

You don’t need to use a special delimiter to close the comment; use the regular comment closing syntax (`*/`) to finish a multiline prose block.

### Reference Localized Prose

Localize the content on a page by using the special comment syntax: `//:#localized(key: `*identifier*`)`. The *identifier* key must correspond to an entry in the playground page’s `Prose.strings` file for each localization folder in the PrivateResources folder.

In the following example, the `ExplanationOfLoops` key refers to localized prose in a page’s `Prose.strings` file, in the en.lproj folder under PrivateResources.

```
//:#localized(key: "ExplanationOfLoops")
```

Strings files (localization files with names ending in `.strings`) contain multiple key-value pairs, where the key is a phrase you use to identify a block of localized prose, and the value is the localized prose.

The example below shows an English localization of `ExplanationOfLoops`.

```
/* An intro to loops. */
"ExplanationOfLoops"="Use loops to repeat an action multiple times until a condition is met.";
```

The rendered playground page shows the text “Use loops to repeat an action multiple times until a condition is met.” If you provide multiple localizations of your playground book, the text displayed is matched to the locale chosen on the learner’s iPad.

Strings files are a common format used for several kinds of localization and internationalization tasks. For more information about formatting strings files, see String Resources and Internationalization and Localization Guide.

## See Also

### Annotations

Specifying Editable Regions in a Playground Page

Guide learning by marking code that learners can change or copy forward.

Hiding Code from a Playground Page

Use special Swift comments to hide code from display but continue to run it.

Customizing the Completions in the Shortcut Bar

Guide learners toward a solution by hiding some symbols and showing others.

Localizing Code Comments and String Literals

In Swift Playgrounds 3.0 and later, mark up code zones to replace them with code that’s localized for the current user.

