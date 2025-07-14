

- ClassKit Catalog API
- Context
- Context.Data
-  Context.Data.ProgressReportingCapabilities 

Dictionary

# Context.Data.ProgressReportingCapabilities

The progress reporting capabilities supported by a context.

ClassKit 1.0+

``` source
object Context.Data.ProgressReportingCapabilities
```

## Properties

`details`

`string`

A description of the capability presented to teachers. See details.

`kind`

`string`

The kind of progress reporting capability. See kind.

Possible Values: `duration, percent, binary, quantity, score`

## Attributes 

Possible types:

## Discussion

When creating a context, if you don’t specify a progress reporting capability with `kind` set to `duration`, the system adds one automatically, using an empty string for the `details` field.

