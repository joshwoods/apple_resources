

- FinanceKit
- TransactionQuery
-  predicate(forMerchantCategoryCodes:) 

Type Method

# predicate(forMerchantCategoryCodes:)

A predicate that returns transactions that match any of the provided merchant category codes.

iOS 17.4+iPadOS 17.4+

``` source
static func predicate(forMerchantCategoryCodes merchantCategoryCodes: [MerchantCategoryCode]) -> Predicate
```

## Parameters 

`merchantCategoryCodes`  

Merchant category codes to match against.

