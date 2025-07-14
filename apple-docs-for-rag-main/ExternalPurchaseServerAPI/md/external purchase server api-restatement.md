

- External Purchase Server API
-  restatement 

Type

# restatement

A Boolean value that indicates a line item contains a correction.

External Purchase Server API 1.0.0+

``` source
boolean restatement
```

## Attributes 

Default: `false`

## Mentioned in 

Reporting corrections

## Discussion

Set this value to `true` to indicate the line item is restating a previously submitted line item, and contains corrections.

Important

Restated line items overwrite the previous submission with the same lineItemId. Be sure to include all the data in the line item, even those fields that are unchanged from the original.

To report erroneously submitted line items, set both the `restatement` and erroneouslySubmitted fields to `true`.

For more information on correcting previously submitted line items, see Reporting corrections.

## See Also

### Submitting corrections

type erroneouslySubmitted

A Boolean value that indicates whether a line item was submitted in error.

