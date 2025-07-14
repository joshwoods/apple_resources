

- Core Spotlight
-  Adding your app’s content to Spotlight indexes 

Article

# Adding your app’s content to Spotlight indexes

Create a description for your app’s content and add it to a Spotlight index to make it searchable.

## Overview

Search makes your app’s content easier to find, and plays a role both inside your app and for features like Spotlight Search, Handoff, Siri Suggestions, Reminders, and more. Making your content searchable enhances the overall user experience of your app and improves the discoverability of your content.

To help search find your content, create a private, on-device index using the Core Spotlight framework and add your app’s data to that index. Search works best when you index content that the person cares about or interacts with directly, such as favorites, items they purchased, messages they sent and received, and so on.

In addition to the content people can see in your UI, enable the isEligibleForSearch property in relevant NSUserActivity objects that your app sends and receives. Enabling this property in user-initiated activities adds those activities to the on-device index and includes them in subsquent searches. For more information, see NSUserActivity.

### Assemble the item attributes

After you identify the content you want to index, collect some details about it. Regardless of whether an item is a file or some part of your app’s data structures, you provide metadata for that item to the Core Spotlight index. You specify this metadata using a CSSearchableItemAttributeSet object, filling out only the properties that make sense for your content. Attribute sets include data for specific types of content, such as images and music. They also contain more general information about an item, such as its name, who created it, the subject matter, and more.

Create the `CSSearchableItemAttributeSet` object and fill in as many properties as makes sense for your data. Attribute sets store simple data types such as strings, numbers, and dates to make the information easier to search. The following example shows a method to index an app-specific data type that manages a spreadsheet document. The code retrieves data from the custom type to fill in the relevant attributes:

```
```

The CSSearchableItemAttributeSetclass supports making a phone call or getting directions to a location associated with an item. To enable these features, set the item’s supportsPhoneCall or supportsNavigation property to `1` and fill in the relevant phone number or latitude and longitude information. Only enable these actions when it’s appropriate and they represent a primary action someone is likely to take. For example, it makes sense to let someone call a business, but it doesn’t make sense to let someone call a phone number that appears on a research paper.

### Create a searchable item to find your content later

With the attributes you collect for each item, create a CSSearchableItem to pass to the indexing system. For each searchable item, specify these details:

- A unique identifier string for locating the item in your app’s data structures

- The attribute set with the item’s metadata

- An optional string that specifies the domain or owner of the item.

Create searchable items as soon as you have the information to do so. When someone creates a new item in your app, create a searchable item for it immediately and add it to the index. When someone changes the title of an item or other details, update the attributes and add it to the index again. It’s very important to keep your app’s indexes up to date so that searches return current information. People are more likely to engage with your app if it returns good search results. A high level of engagement also helps increase the ranking of your searchable items.

The following code builds on the previous example by creating a searchable item for a custom app data structure. The code uses data from the data item itself to fill in various attributes.

```
```

If you expect an item to exist for an extended period of time, set an appropriate value in the item’s expirationDate property. The system automatically expires items after a period of time, so setting an expiration date causes the system to preserve the item until the date you specify. If the person deletes the original data from your app, remove the associated item from the index.

### Add items to a searchable index

To make your items appear in search results, add them to a CSSearchableIndex object. Indexes store your app-specific data and remain on the device. You can create multiple indexes for your app, and might do so to protect someone’s personal information. For example, a music app might place the general catalog of songs in the default index and someone’s private playlists in an encrypted index.

The default `CSSearchableIndex` object supports the indexing of items that don’t require special protection. When indexing content that contains more sensitive data, such as someone’s contact information, create a more secure index using the init(name:protectionClass:) method. The following example creates a secure index in addition to retrieving the default index for data that doesn’t require any specific protections:

```
```

To add new items to an index, or to update items already in an index, call the indexSearchableItems(_:completionHandler:) method of that index. The method incorporates the items asynchronously into the index and notifies you when the work is done. Typically, you submit items only when they change, but you might also submit items to extend their expiration date.

```
```

Important

Provide a reindexing app extension to keep the index up to date even when your app isn’t running. For more information, see Regenerating your app’s indexes on demand.

### Add multiple items to the index in batches

When adding or updating large numbers of items, consider breaking those updates into multiple batches. Batch updates make it easier for your code to recover from errors or crashes that happen during the indexing process. The system waits for you to specify your searchable items and end the batch update before it begins indexing the items. If an error occurs, the metadata you add to the batch lets you determine the extent of the indexing progress, and where the error occurred.

Note

The default() index doesn’t support batch operations.

The following example shows a function that indexes several items using a batch update. You can specify any information you want for the client data, but must limit the total size of it to 250 bytes. If any errors occur during the batch update, you can call fetchLastClientState(completionHandler:) to determine where to start indexing your content again.

```
```

## See Also

### Essentials

Enabling Apple Intelligence summarization and prioritization

Summarize and prioritize app content using Spotlight extensions.

