# Example Queries

##First order Income Accounts with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  

WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>  
WHERE{
?Item rdf:type elod:SpendingItem ;
dcterms:issued ?date.
?Item elod:seller <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
}
GROUP BY ?kaeuri
}

}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)

##First order Expense Accounts with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  

WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>
where{
?Item rdf:type elod:SpendingItem ; dcterms:issued ?date.
?Item elod:buyer <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
}
GROUP BY ?kaeuri
}

}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)
LIMIT 50

##Property Accounts with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  

WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>  
WHERE{
?Item rdf:type elod:SpendingItem ;
dcterms:issued ?date.
?Item elod:seller <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
FILTER ((STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/1") && !STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/1/12")&& !STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/1/13"))|| (STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2") &&!STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2111") &&!STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2112") &&!STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2113") &&!STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2114") &&!STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2116")) ) .     
}
GROUP BY ?kaeuri
}

}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)

##Retaliatory Revenue with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  
WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>  
WHERE{
?Item rdf:type elod:SpendingItem ;
dcterms:issued ?date.
?Item elod:seller <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
FILTER  (STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/0/03") ||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/0/04/047")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/0/05/053")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2111")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2112")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2113")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2114")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/2/21/211/2116")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/3/32/321/3211")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/3/32/321/3212")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/3/32/321/3213")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/3/32/321/3214")||
STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Income/3/32/321/3216"))         
}
GROUP BY ?kaeuri
}

}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)

##Loan Accounts with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  

WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>
where{
?Item rdf:type elod:SpendingItem ; dcterms:issued ?date.
?Item elod:buyer <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
FILTER  (STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Expense/6/65")) .
}
GROUP BY ?kaeuri
}

}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)

##Investment Accounts with their amounts for year 2015

SELECT ?kaeuri ?nameOfKae ?sum
FROM <<http://linkedeconomy.org/ThessBudget>>  

WHERE{
{
SELECT ?kaeuri (MAX(?nameOfKae) as ?nameOfKae)
FROM <<http://linkedeconomy.org/Budgets/KAE>>
WHERE {
OPTIONAL {?kaeuri rdfs:label ?nameOfKae .}
FILTER(langMatches(lang(?nameOfKae), "en")).
}
GROUP BY ?kaeuri
}
{
SELECT ?kaeuri (sum(xsd:decimal(?amount)) as ?sum)
FROM <<http://linkedeconomy.org/ThessBudget>>
where{
?Item rdf:type elod:SpendingItem ; dcterms:issued ?date.
?Item elod:buyer <<http://linkedeconomy.org/resource/Organization/998082845>>.
?Item elod:hasExpenditureLine ?expline.
?expline elod:amount ?ups.
?expline elod:hasKae ?kaeuri.
?ups gr:hasCurrencyValue ?amount .
FILTER (?date = "2015-12-31"^^xsd:date) .
FILTER  (STRSTARTS(STR(?kaeuri), "http://linkedeconomy.org/resource/KAE/2015/Expense/7") ) .
}
GROUP BY ?kaeuri
}
}
GROUP BY ?kaeuri
ORDER BY DESC (?sum)


