

- Swift Playgrounds
-  Localizing a Subscription Feed 

Article

# Localizing a Subscription Feed

Provide multiple localizations of a subscription’s content in a single feed.

## Overview

You can provide localizations of your subscription content by linking to a supplemental JSON object that maps locale IDs to locale-specific feeds.

### Create the Localization Mapping in JSON

Each localization of your subscription’s content requires its own entry in the supplemental JSON object. You create the mapping from a locale ID—a standard format described in Locale IDs—to the localized feed URL by pairing the two for that locale. You use the locale ID as the key and the localized feed URL as the value for each key-value pair in the JSON object.

For example, you can supply the following locale JSON to support a feed that’s localized to contain English and French versions of a subscription’s content:

```
```

The locale ID for the French localization is `fr`, and `fr-feed.json` contains French metadata and the URL for the localized French playground books in the subscription.

### Share the Localized JSON Object’s URL

Unlike feeds that aren’t localized, localized feeds download the supplemental JSON object as an extra step to determine locale information before downloading your feed’s content. As a result, you need to use the URL for the supplemental JSON object when sharing your subscription.

## See Also

### Subscriptions

Creating a subscription

Create a machine-readable summary of a set of playground books to make them available for others to download.

Publishing a Subscription

Make the playground books in a series available online for download and subscription.

