

- TVMLKit JS
- LoadIndexesRequest
-  close 

Instance Method

# close

Signals whether or not the data fetch is successful.

tvOS 13.0+

``` source
void close(
    in Boolean success
);
```

## Discussion

The Boolean value passed into the `close` method signals whether or not the data fetch succeeded. If true is passed, then those indexes are marked internally as loaded, and a loadindexes event for these indexes won't be invoked again. If false is passed, the loadindexes event will be invoked only when those indexes are needed again.

