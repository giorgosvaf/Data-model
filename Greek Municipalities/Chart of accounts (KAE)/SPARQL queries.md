# Example Queries

### Query results can be retrieved by [this google spreadsheet] (https://drive.google.com/open?id=10DyKiU2ACOuugbop8NMTYsi1p0fZCjkBBH6Qx_jGtpI).

##First Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeTwoDigits ?twoDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER (STR(?twoDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Second Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
 elod:kaeTwoDigits ?twoDigits ;
elod:kaeThreeDigits ?threeDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER (STR(?twoDigits)!= "no digit").
FILTER (STR(?threeDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Third Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeThreeDigits ?threeDigits;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER (STR(?threeDigits)!= "no digit").
FILTER (STR(?fourDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Fourth Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER (STR(?fourDigits)!="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Revenue First Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeTwoDigits ?twoDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Income").
FILTER (STR(?twoDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Revenue Second Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
 elod:kaeTwoDigits ?twoDigits ;
elod:kaeThreeDigits ?threeDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Income").
FILTER (STR(?twoDigits)!= "no digit").
FILTER (STR(?threeDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Revenue Third Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeThreeDigits ?threeDigits;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Income").
FILTER (STR(?threeDigits)!= "no digit").
FILTER (STR(?fourDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Revenue Fourth Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Income").
FILTER (STR(?fourDigits)!="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Expense First Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeTwoDigits ?twoDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Expense").
FILTER (STR(?twoDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Expense Second Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
 elod:kaeTwoDigits ?twoDigits ;
elod:kaeThreeDigits ?threeDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Expense").
FILTER (STR(?twoDigits)!= "no digit").
FILTER (STR(?threeDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Expense Third Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeThreeDigits ?threeDigits;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Expense").
FILTER (STR(?threeDigits)!= "no digit").
FILTER (STR(?fourDigits)="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Expense Fourth Level KAEs for year 2015

SELECT ?KAEUri ?nameOfKAE  
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?KAEUri rdfs:label ?nameOfKAE;
elod:kaeFourDigits ?fourDigits.
FILTER REGEX (STR(?KAEUri),"2015").
FILTER REGEX (STR(?KAEUri),"Expense").
FILTER (STR(?fourDigits)!="no digit").
FILTER(langMatches(lang(?nameOfKAE), "en")).
}

## Sub - KAEs of  Category of KAE “0 - INCOME”

SELECT ?subKaeCode ?nameOfSubKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
<<http://linkedeconomy.org/resource/KAE/2015/Income/0>> elod:hasSubKaeCode ?subKaeCode.
?subKaeCode rdfs:label ?nameOfSubKaeCode .
FILTER(langMatches(lang(?nameOfSubKaeCode), "en")).
}

## Sub - KAEs of Group of KAE “01 - REVENUE FROM REAL ESTATE”

SELECT ?subKaeCode ?nameOfSubKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
<<http://linkedeconomy.org/resource/KAE/2015/Income/0/01>> elod:hasSubKaeCode ?subKaeCode.
?subKaeCode rdfs:label ?nameOfSubKaeCode .
FILTER(langMatches(lang(?nameOfSubKaeCode), "en")).
}

## Sub - KAEs of Type of KAE “011 - RENTALS”

SELECT ?subKaeCode ?nameOfSubKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
<<http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011>> elod:hasSubKaeCode ?subKaeCode.
?subKaeCode rdfs:label ?nameOfSubKaeCode .
FILTER(langMatches(lang(?nameOfSubKaeCode), "en")).
}

## Super - Kae of Type of KAE “60 - WAGES AND STAFF EXPENSES”

SELECT ?superKaeCode ?nameOfSuperKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?superKaeCode elod:hasSubKaeCode <<http://linkedeconomy.org/resource/KAE/2015/Expense/6/60>>.
?superKaeCode rdfs:label ?nameOfSuperKaeCode .
FILTER(langMatches(lang(?nameOfSuperKaeCode), "en")).
}

## Super - Kae of Type of KAE “601 - SALARIES OF PERMANENT OFFICIALS”

SELECT ?superKaeCode ?nameOfSuperKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?superKaeCode elod:hasSubKaeCode <<http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601>>.
?superKaeCode rdfs:label ?nameOfSuperKaeCode .
FILTER(langMatches(lang(?nameOfSuperKaeCode), "en")).
}

## Super - Kae of Detailed Type of KAE “6011 - Regular salaries”

SELECT ?superKaeCode ?nameOfSuperKaeCode
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
?superKaeCode elod:hasSubKaeCode <<http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601/6011>>.
?superKaeCode rdfs:label ?nameOfSuperKaeCode .
FILTER(langMatches(lang(?nameOfSuperKaeCode), "en")).
}

