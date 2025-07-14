

- Swift Playgrounds
- Playground Books
-  Giving hints to help learners solve problems 

Article

# Giving hints to help learners solve problems

Add hints, spoilers, and solutions to a page to help teach the material.

## Overview

Learners sometimes become stuck when working through a challenge or learning assessment. Try to anticipate where learners are likely to become stuck when going through your playground book, and provide hints to help them.

Hints are disclosed after the learner taps the Hint button in a page’s live view.

### Add hints by using a property list

Add hints to your playground page by creating a property list at the following path, alongside the rest of the resources for the page:

*\*`.playgroundbook/Contents/`*\*`.playgroundchapter/Pages/`*\*`.playgroundpage/PrivateResources/Hints.plist`

The root key for the hints property list is named `Hints`, and it must contain an array of dictionaries. Hints are shown in Swift Playgrounds in the same order as they appear in this array.

### Add keys to the dictionaries

Add the following keys in each dictionary in the hints array:

`Content`  
The text of the hint.

`FileReference`  
The path to a text file that contains the hint. This path is relative to the page’s Resources folder, so a hint file located at the following path only needs to be referenced as `MyHint.txt` in the value of the `FileReference` key:

`.playgroundbook/Contents/``.playgroundchapter/Pages/``.playgroundpage/PrivateResources/MyHint.txt`

`SpoilerButtonTitle`  
A hint that’s hidden until the learner taps a button. Include the `SpoilerButtonTitle` key to hide the hint. The string you supply as the value for the key becomes the button’s title.

Don’t include both the `Content` and `FileReference` keys in the same dictionary. You can use either one, but not both, because they both serve the role of provider of the hint text.

You can use markup to format hint text. For more information, see Markup Formatting Reference.

### Create hints for various contexts

Create hints, spoilers, and solutions to suit the needs of each of your playground pages. The example below shows each of the forms a hint can take.

```

    Hints

            Content
            Look at the `characters` property of `String`.

            Content
            This hint is initially hidden by a spoiler button.
            SpoilerButtonTitle
            Show Spoiler

            FileReference
            OutOfBandHint.txt

            FileReference
            OutOfBandHintWithSpoilerButton.txt
            SpoilerButtonTitle
            Show Spoiler

```

Here’s how the hints property list looks when displayed as a popover in the playground page’s live view:

