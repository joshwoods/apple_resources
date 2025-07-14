

- Core Services
- Search Kit
- Text Analysis Keys
-  kSKMaximumTerms 

Global Variable

# kSKMaximumTerms

macOS 10.4+

``` source
let kSKMaximumTerms: CFString!
```

## Discussion

The maximum number of number unique terms to index in each document. Specified as a CFNumber object.

Search Kit indexes from the beginning of a document. When it has indexed the first n unique terms, it stops.

The default number of maximum terms, which applies if you do not provide a number, is 2000.

To tell Search Kit to index all the terms in each document without limit, specify a value of 0.

