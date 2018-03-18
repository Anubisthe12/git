.. _relyingparties:

JavaScript
###############

- metódy s array

Modifikačné metódy 
==========

var pole = ["1","2","3","4","5"];
=> pole.pop(); 

* pop() 
 - odstraňuje posledný prvok poľa, vracia pole
["1","2","3","4"] 
* shift() 
- odstraňuje posledný prvok poľa, vracia odstránený prvok
 ["1","2","3","4"] 
návratová hodnota - "5"

* push() 
- pridáva posledný prvok poľa
=> ["1","2","3","4","5","Pridaný prvok"];
* unshift()
- pridáva prvé prvky poľa, vracia dĺžku poľa
=> ["Pridaný prvok","1","2","3","4","5"];
=> návratová hodnota - 6
* reverse() 
- obráti prvky poľa
=> ["5", "4", "3", "2", "1"]
* sort() 
- zoradenie prvkov
=> ["1","2","3","4","5"]
* splice() 
- pridavanie a odstranovanie prvkov
- pole.splice(1,2,"Pridaný prvok")
- (ktorý prvok -indexové poradie, koľko prvkov, nový prvok)
=> ["1", "Pridaný prvok", "4", "5"]

Prístupové metódy
==========
* concat()
* join()
* slice()
* toString
* indexOf()
* lastIndexOf()

Iteračné metódy
==========
* foreach()
* map()
* every()
* some()
* filter()
* reduce() a reduceRight()
