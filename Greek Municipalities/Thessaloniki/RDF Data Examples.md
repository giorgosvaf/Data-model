##RDF Data Examples

###RDF example for input data of Budget Thessaloniki
```xml
  <http://linkedeconomy.org/resource/BudgetItem/2015/31-12/0/01/011/0111/1> a elod:BudgetItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/BudgetItem/2015/31-12/0/01/011/0111/1>;
	    elod:seller <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued "2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΜΙΣΘΩΜΑΤΑ ΑΠΟ ΑΝΘΟΠΩΛΕΙΑ ΝΕΩΝ ΚΟΙΜΗΤΗΡΙΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/BudgetItem/2015/31-12/0/01/011/0111/1> 
			elod:price [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "128000.00"^^xsd:float;
                       ]
					   
  <http://linkedeconomy.org/resource/ExpenseApprovalItem/2015/31-12/0/01/011/0111/1> a elod:ExpenseApprovalItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/0/01/011/0111/1>;
	    elod:seller <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΜΙΣΘΩΜΑΤΑ ΑΠΟ ΑΝΘΟΠΩΛΕΙΑ ΝΕΩΝ ΚΟΙΜΗΤΗΡΙΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/0/01/011/0111/1> 
			elod:amount [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "117185.00"^^xsd:float;
                       ]
					   
  <http://linkedeconomy.org/resource/SpendingItem/2015/31-12/0/01/011/0111/1> a elod:SpendingItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/SpendingItem/2015/31-12/0/01/011/0111/1>;
	    elod:seller <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΜΙΣΘΩΜΑΤΑ ΑΠΟ ΑΝΘΟΠΩΛΕΙΑ ΝΕΩΝ ΚΟΙΜΗΤΗΡΙΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/SpendingItem/2015/31-12/0/01/011/0111/1> 
			elod:amount [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "117185.00"^^xsd:float;
                       ]

  <http://linkedeconomy.org/resource/BudgetItem/2015/31-12/6/60/601/6011/1> a elod:BudgetItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/BudgetItem/2015/31-12/6/60/601/6011/1>;
	    elod:buyer <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΤΑΚΤΙΚΕΣ ΑΠΟΔΟΧΕΣ ΜΟΝΙΜΩΝ ΥΠΑΛΛΗΛΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/BudgetItem/2015/31-12/6/60/601/6011/1> 
			elod:price [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "1400000.00"^^xsd:float;
                       ]
					   
 <http://linkedeconomy.org/resource/CommittedItem/2015/31-12/6/60/601/6011/1> a elod:CommittedItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/6/60/601/6011/1>;
	    elod:buyer <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΤΑΚΤΙΚΕΣ ΑΠΟΔΟΧΕΣ ΜΟΝΙΜΩΝ ΥΠΑΛΛΗΛΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/6/60/601/6011/1> 
			elod:amount [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "1400000.00"^^xsd:float;
                       ]					   
					   
  <http://linkedeconomy.org/resource/ExpenseApprovalItem/2015/31-12/6/60/601/6011/1> a elod:ExpenseApprovalItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/6/60/601/6011/1>;
	    elod:buyer <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΤΑΚΤΙΚΕΣ ΑΠΟΔΟΧΕΣ ΜΟΝΙΜΩΝ ΥΠΑΛΛΗΛΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/ExpenseApprovalItem/2015/31-12/6/60/601/6011/1> 
			elod:amount [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "1380198.43"^^xsd:float;
                       ]
					   
  <http://linkedeconomy.org/resource/SpendingItem/2015/31-12/6/60/601/6011/1> a elod:SpendingItem ;
		elod:hasExpenditureLine <http://linkedeconomy.org/resource/ExpenditureLine/SpendingItem/2015/31-12/6/60/601/6011/1>;
	    elod:buyer <http://linkedeconomy.org/resource/Organization/998082845>;
		dcterms:issued 	"2015-12-31+02:00"^^xsd:dateTime;
		elod:financialYear "2015"^^xsd:gYear;
		dcterms:subject "ΤΑΚΤΙΚΕΣ ΑΠΟΔΟΧΕΣ ΜΟΝΙΜΩΝ ΥΠΑΛΛΗΛΩΝ"^^xsd:string.
		<http://linkedeconomy.org/resource/ExpenditureLine/SpendingItem/2015/31-12/6/60/601/6011/1> 
			elod:amount [ a gr:UnitPriceSpecification;
			             elod:hasCurrency <http://linkedeconomy.org/resource/Currency/EUR>;
			             gr:hasCurrencyValue "1380198.43"^^xsd:float;
                       ]
					   
