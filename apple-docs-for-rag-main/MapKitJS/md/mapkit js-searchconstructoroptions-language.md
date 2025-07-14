

- MapKit JS
- SearchConstructorOptions
-  language 

Instance Property

# language

A language ID that determines the language for the search results text.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

If you set a language ID, the search returns addresses in the selected language, if available, such as, `fr-CA` or `en-GB`. If you don’t provide a language ID, the search object uses the language ID the system provides to the init call.

## See Also

### Search Initialization

coordinate

A map coordinate that provides a hint for the geographic area to search.

getsUserLocation

A Boolean value that indicates whether to limit the search results to the user’s location, according to the web browser.

region

A map region that provides a hint for the geographic area to search.

