

- External Purchase Server API
-  erroneouslySubmitted 

Type

# erroneouslySubmitted

A Boolean value that indicates whether a line item was submitted in error.

External Purchase Server API 1.0.0+

``` source
boolean erroneouslySubmitted
```

## Attributes 

Default: `false`

## Mentioned in 

Reporting corrections

## Discussion

Only use this field when submitting corrections to a report. Set this field to `true` to indicate that you previously submitted the line item erroneously. This effectively undoes the line item submission. When submitting a correction, set the restatement field to `true`.

For more information on correcting previously submitted line items, see Reporting corrections.

## See Also

### Submitting corrections

type restatement

A Boolean value that indicates a line item contains a correction.

