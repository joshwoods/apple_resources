

- Apple Music API
- RecordLabels
- RecordLabels.Views
-  RecordLabels.Views.RecordLabelsTopReleasesView 

Object

# RecordLabels.Views.RecordLabelsTopReleasesView

A relationship view from this record label to a selection of its top releases.

Apple Music 1.0+

``` source
object RecordLabels.Views.RecordLabelsTopReleasesView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

RecordLabels.Views.RecordLabelsTopReleasesView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`Albums`]`

 (Required) 

A selection of top releases from this record label.

## Topics

### Related Objects

object RecordLabels.Views.RecordLabelsTopReleasesView.Attributes

The attributes for the record label top releases view.

## See Also

### Related Objects

object RecordLabels.Views.RecordLabelsLatestReleasesView

A relationship view from this record label to a selection of its latest releases.

