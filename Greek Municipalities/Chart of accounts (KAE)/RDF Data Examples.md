##RDF Data Examples

###RDF example for input data of KAE
```xml
  <http://linkedeconomy.org/resource/KAE/2015/Income/0> a elod:KAE ;
        rdfs:label "ΤΑΚΤΙΚΑ ΕΣΟΔΑ"@el;
		rdfs:label "INCOME"@en;
        elod:kaeOneDigit "0"^^xsd:string;
        elod:kaeTwoDigits "no digit"^^xsd:string;
		elod:kaeThreeDigits "no digit"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Income>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/02>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/03>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/03>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/04>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/05>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/06>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/07>.
				
  <http://linkedeconomy.org/resource/KAE/2015/Income/0/01> a elod:KAE ;
        rdfs:label "ΠΡΟΣΟΔΟΙ ΑΠΟ ΑΚΙΝΗΤΗ ΠΕΡΙΟΥΣΙΑ"@el;
		rdfs:label "REVENUE FROM REAL ESTATE"@en;
        elod:kaeOneDigit "0"^^xsd:string;
        elod:kaeTwoDigits "01"^^xsd:string;
		elod:kaeThreeDigits "no digit"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Income>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/012>.
		
  <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011> a elod:KAE ;
        rdfs:label "ΜΙΣΘΩΜΑΤΑ"@el;
		rdfs:label "RENTALS"@en;
        elod:kaeOneDigit "0"^^xsd:string;
        elod:kaeTwoDigits "01"^^xsd:string;
		elod:kaeThreeDigits "011"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Income>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0111>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0112>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0113>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0114>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0115>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0116>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0117>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0118>>.
		
  <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011/0111> a elod:KAE ;
        rdfs:label "Μισθώματα από αστικά ακίνητα (άρθρο 192 ΚΔΚ)"@el;
		rdfs:label "Rentals of residential real estate"@en;
        elod:kaeOneDigit "0"^^xsd:string;
        elod:kaeTwoDigits "01"^^xsd:string;
		elod:kaeThreeDigits "011"^^xsd:string;
		elod:kaeFourDigits "0111"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Income>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Income/0/01/011>.
		
  <http://linkedeconomy.org/resource/KAE/2015/Expense/6> a elod:KAE ;
        rdfs:label "ΕΞΟΔΑ ΧΡΗΣΗΣ"@el;
		rdfs:label "USE EXPENDITURE"@en;
        elod:kaeOneDigit "6"^^xsd:string;
        elod:kaeTwoDigits "no digit"^^xsd:string;
		elod:kaeThreeDigits "no digit"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Expense>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/61>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/62>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/63>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/64>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/65>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/66>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/67>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/68>.

  <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60> a elod:KAE ;
        rdfs:label "ΑΜΟΙΒΕΣ ΚΑΙ ΕΞΟΔΑ ΠΡΟΣΩΠΙΚΟΥ"@el;
		rdfs:label "WAGES AND STAFF EXPENSES"@en;
        elod:kaeOneDigit "6"^^xsd:string;
        elod:kaeTwoDigits "60"^^xsd:string;
		elod:kaeThreeDigits "no digit"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Expense>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6>
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/602>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/603>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/604>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/605>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/606>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/607>.
		
  <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601> a elod:KAE ;
        rdfs:label "ΑΠΟΔΟΧΕΣ ΜΟΝΙΜΩΝ ΥΠΑΛΛΗΛΩΝ"@el;
		rdfs:label "SALARIES OF PERMANENT OFFICIALS"@en;
        elod:kaeOneDigit "6"^^xsd:string;
        elod:kaeTwoDigits "60"^^xsd:string;
		elod:kaeThreeDigits "601"^^xsd:string;
		elod:kaeFourDigits "no digit"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Expense>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60>
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601/6011>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601/6012>;
		elod:hasSubKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601/6013.
		
  <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601/6011> a elod:KAE ;
        rdfs:label "Τακτικές αποδοχες (περιλαμβάνονται βασικός μισθός, δώρα εορτών, γενικά και ειδικά τακτικά επιδόματα)"@el;
		rdfs:label "Regular salaries"@en;
        elod:kaeOneDigit "6"^^xsd:string;
        elod:kaeTwoDigits "60"^^xsd:string;
		elod:kaeThreeDigits "601"^^xsd:string;
		elod:kaeFourDigits "6011"^^xsd:string;
		elod:hasKind <http://linkedeconomy.org/resource/KaeKind/Expense>;
		elod:hasSuperKaeCode <http://linkedeconomy.org/resource/KAE/2015/Expense/6/60/601>.
