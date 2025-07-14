

- Wallet Passes
-  Creating the Source for a Pass 

Article

# Creating the Source for a Pass

Create the directory structure and add source files and images to define a pass.

## Overview

The source for your pass includes all the information the system needs to show it to the user:

- Image files for the icon and other visual elements, such as a logo.

- A `pass.json` file that contains the strings the system displays on the pass and the metadata that defines the pass.

- Optional localization information.

Create the source in a directory that you use to create the final distributable pass Bundle. For information on building a pass from the source, see Building a Pass.

### Create the Directory and add Files for the Pass

First create a directory to hold all the source files. The name of the directory is the name of the final pass file followed by `.pass`. For example, `Lift It Membership.pass` is the name of the top-level directory for the source of the Lift It membership pass.

Add the `pass.json` file that contains the information and metadata for the pass. For more information on the contents of this file, see the top-level Pass object.

The following figure shows the directory structure for a simple pass that’s localized for English and Simplified Chinese:

### Add the images for the Pass

Customize the look of your pass by using images for a logo and other items. All passes require an icon:

- In notifications, including on the lock screen.

- As the image for an email attachment.

Some types of passes include other types of images, such as a background. For more information, see Pass Design and Creation.

### Add Localization to the Pass

Expand your audience by localizing the strings and images of your pass to different languages and regions.

Add a directory at the top-level source directory of each pass for each localization. The name of the directory identifies the language and an optional region:

`[language identifier]-[region identifier].lproj`

For example, the name for the French localization directory is `fr.lproj`, and the name for the Simplified Chinese directory is `zh-Hans.lproj`. For more information on language identifiers, see `Understand the Language Identifier`.

Localize an image by adding the location-specific image files to each localization directory. For example, to add the localized versions of the diamond logo shown above, add the English version of the `logo@2x.png` and `logo@3x.png` files to the `en.lproj` folder and the Chinese version of the `logo@2x.png` and `logo@3x.png` files to the `zh-Hans.lproj` folder. Each folder must contain the same number of resolutions for an image.

Note

Adding an image of the same name to the top-level folder of the pass overrides any localized versions. In addition, the localized image of a pass may not update after adding the pass to Wallet.

### Localize the Strings

When a user opens a pass, the system localizes displayed strings in two different ways. The system localizes pass fields that contain dates, times, and currencies that use standard formats in the `pass.json` file. For example, in the pass shown above, the expiration date value is an ISO 8601 date in PassFieldContent:

```
{
   "dateStyle": "PKDateStyleShort", 
   "isRelative": true, 
   "key": "expires", 
   "label": "ExpiresLabel", 
   "value": "2019-06-26T12:00:00+00:00"
}
```

The system always displays localized versions of these values, even when your pass doesn’t contain localization folders for the language. For example, the figure below shows a pass that contains localizations for English and Simplified Chinese displayed on a device set to the Arabic language. The system only localizes the date:

The system localizes other strings on your pass using a *strings file* which contains a list of keys and associated localized strings. Add localized strings to your pass in three steps:

- Set the value of a displayed string in `pass.json` to a key, such as `“OfferAmountLabel”` for the `label` of the offer amount field.

- Add a `pass.strings` file to the localization folder.

- Add a line to each `pass.strings` file that sets a key you created in `pass.json` to the localized term.

For example, the following three code snippets show the code to localize the offer label and offer text of the passes shown above to English and to Simplified Chinese.

Set the value of the strings in the PassFields.PrimaryFields object in the `pass.json` file to the keys you use to show a localized string in the `pass.strings` files`:`

```
...  
   "primaryFields": [
      {
        "key": "offer", 
        "value": "OfferAmount"
        "label": "OfferAmountLabel", 
      }
    ]
...
```

Set the English strings in `en.lproj/pass.strings`:

```
/* English Localization */
/* Offer strings */
"OfferAmount" = "100% off";
"OfferAmountLabel" = "Anything you want!";
```

Set the Simplified Chinese strings in `zh-Hans.lproj/pass.strings`:

```
/* Simplified Chinese Localization */
/* Offer strings */
"OfferAmount" = "100% 折扣";
"OfferAmountLabel" = "尽享所需一切！";
```

Use UTF-16 encoding for non-ASCII characters.

## See Also

### Essentials

Building a Pass

Build a distributable pass.

Distributing and updating a pass

Distribute a pass to your users or update an existing pass.

object Pass

An object that represents a pass.

