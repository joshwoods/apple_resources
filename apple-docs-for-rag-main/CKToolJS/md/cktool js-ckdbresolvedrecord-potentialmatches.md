

- CKTool JS
- CKDBResolvedRecord
-  potentialMatches 

Instance Property

# potentialMatches

An array of potential participants that the user can choose from.

CKTool JS 1.2.15+

``` source
attribute CKDBSharePotentialParticipant[]? potentialMatches;
```

## Discussion

This array only contains values if the participant is not identifiable. If this array is populated, each value is a `CKDBSharePotentialParticipant` object.

