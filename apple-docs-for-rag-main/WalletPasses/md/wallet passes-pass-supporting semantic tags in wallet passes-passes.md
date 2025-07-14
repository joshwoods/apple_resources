

- Wallet Passes
- Pass
-  Supporting semantic tags in Wallet passes 

Article

# Supporting semantic tags in Wallet passes

Enable the system to offer suggestions for actions related to passes by adding machine-readable metadata.

## Overview

You can augment the user-visible information on Wallet passes with machine-readable metadata known as *semantic tags*. The metadata in semantic tags helps the system better understand Wallet passes and suggest relevant actions for the user to take on their installed passes.

You can add semantic tags to all types of Wallet passes, but some tags only apply to specific types, such as event tickets, boarding passes, and store cards. For a full list of all tags and their associated pass types, see SemanticTags.

### Add semantic tags

To add machine-readable semantic tags to Wallet passes, add a `semantics` dictionary at the root of the Pass dictionary or as a top-level key in any of these dictionaries:

- PassFields.HeaderFields

- PassFields.PrimaryFields

- PassFields.SecondaryFields

- PassFields.AuxiliaryFields

- PassFields.BackFields

The operating system uses the semantic tag data to offer suggestions for actions related to a relevant pass. For example, semantic tags in a movie pass could take effect when the user arrives in the theater at the scheduled time, offering a Siri suggestion to enable Do Not Disturb mode for the duration of the film.

For the system to send the suggestion to set Do Not Disturb, you must set `eventType` to indicate that the pass is a movie ticket, and add these semantic tags:

- `silenceRequested`

- `eventStartDate`

- `eventEndDate`

- `venueLocation`

You can add semantic data to the Pass dictionary in a single `semantictags` dictionary, like this:

```
```

Alternatively, you can add semantic data to enhance the individual fields in a pass. For example, you could add the `eventType` and `silenceRequested` keys to a `semantics` dictionary in the top-level Pass dictionary:

```
```

Then, because the primary field on this movie ticket pass shows the event and venue details, you could add the `eventName`, `venueName`, and `venueLocation` keys to the `semantics` dictionary in PassFields.PrimaryFields:

```
```

A secondary field on this pass shows the length of the movie. Add the `eventStartDate` and `eventEndDate` keys to represent that information semantically:

```
```

Where you choose to add the semantic tags, whether to the top-level Pass dictionary or to a field dictionary, doesn’t affect their functionality. Add them wherever is most convenient when generating your passes.

For the best user experience with your passes, add as much semantic data as you have for all possible semantic tags.

## See Also

### Adding system suggestions

object SemanticTags

An object that contains machine-readable metadata the system uses to offer a pass and suggest related actions.

object SemanticTagType

A compilation of data object types for semantic tags.

