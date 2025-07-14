

- Apple News API
-  Section 

Object

# Section

See the fields the section endpoints returned.

Apple News API 1.0+

``` source
object Section
```

## Properties

`createdAt`

`date-time`

The date and time this section was created.

`id`

`uuid`

The unique identifier of the specified section.

`isDefault`

`boolean`

A Boolean value that indicates whether this is the default section for the channel.

Default: `false`

`modifiedAt`

`date-time`

The date and time this section was last modified.

`name`

`string`

The name of the section.

`shareUrl`

`string`

The URL of the channel in which this section appears.

`type`

`string`

The section.

## Relationships

### Inherited By

- SectionResponse

## See Also

### Sections

List All Sections

See a list of available sections in your channel.

Read Section Information

Get information about the specified section, including its name, its channel, and whether it’s a default section.

Promote Articles in a Section

Set the list of promoted articles for the specified section.

object SectionLinks

See the links the section endpoints returned.

object SectionResponse

See which objects make up the section response.

object PromoteArticleRequest

See the required field for the Promote an Article request.

object PromoteArticleResponse

See the field the Promote an Article response returned.

