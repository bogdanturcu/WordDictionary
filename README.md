# WordDictionary
Introducere:
In cadrul proiectului pentru Cloud Computing am hotarat sa dezvolt o aplicatie simpla si functionala pentru unul din micile incovenente pe care le-am intalnit pe Internet.

Descrierea problemei:

Exista anumite situatii in care caut sensul unui cuvant, definitia, poate un exemplu cu respectivul cuvant, pronuntia sau chiar si "the urban meaning" al cuvantului sau chiar pe toate deodata. Astfel, prin intermediul unei pagini web un utilizator oarecare (inclusiv eu ☺) isi poate cauta cuvantul de interes si sa obtina informatii legate de cuvantul dorit. (Dictionarul este destinat exclusiv pentru cuvinte in limba engleza)

Descriere API:

Pentru aceasta aplicatie am folosit wordnik care la momentul de fata este cel mai mare dictionar in limba engleza ca numar de cuvinte.
Wordnik afiseaza definitii din mai multe surse, astfel incat sa putem vedea cat mai multe explicatii diferite cu privire la semnificatia unui cuvant.
Avand in vedere ca wordnik foloseste mai multe surse pentru preluarea definitilor/exemplelor precum Wiktionary, Wordnet 3.0, GCIDE, The American Heritage® Dictionary of the English Language, Fourth Edition sau The Century Dictionary and Cyclopedia putem sa gasim pentru fiecare search al unor cuvinte definitii sau explicatii diferite unele dintre ele chiar si amuzante(Fiind explicat un sens urban sau de tip jargon al cuvantului. 
(ex: Pig = Any of various mammals of the family Suidae, having short legs, hooves with two weight-bearing toes, bristly hair, and a cartilaginous snout used for digging, including the domesticated hog SAU Pig = Any police officer). 
Cum orice plus are de regula si un drawback daca cautam destul putem gasi cuvinte ca nu au o definitie prestabilita. 
API-ul necesita key care poate sa fie obtinuta pe gratis prin creearea unui cont pe site-ul https://developer.wordnik.com/
![image](https://user-images.githubusercontent.com/72883464/117491531-fcf84f00-af78-11eb-84c0-298292bedab4.png)

Flux de date:

In cadrul acestei aplicatii, cuvantul cautat este preluat prin document.getElementById('searchBox').value apoi, functia face 3 request-uri XMLHttp de tip GET pentru a obtine Definitia, Exemplul si Pronuntia acestea fiind JSON. Datele sunt apelate si manipulate in fisierul index.html, ca in final, utilizatorul sa poata accesa public datele printr-o metoda HTTP.

![image](https://user-images.githubusercontent.com/72883464/117498576-a5f77780-af82-11eb-956b-19c1b0dfa7b6.png)

![image](https://user-images.githubusercontent.com/72883464/117498677-c9222700-af82-11eb-86fb-fbb46115ba4f.png)


Ca "poveste" a acestei aplicatii am parcus urmatorii pasi:
-> Am gasit API-ul pe internet
-> Am folosit Cloud 9 ca mediu de dezvoltare
-> Am folosit Heroku pentru "a face apicatia acesibila"

![image](https://user-images.githubusercontent.com/72883464/117498179-1f429a80-af82-11eb-8a4e-7e6f7c856f9f.png)

![image](https://user-images.githubusercontent.com/72883464/117499349-c70c9800-af83-11eb-95ad-15ca8ed543ce.png)

![image](https://user-images.githubusercontent.com/72883464/117498417-72b4e880-af82-11eb-8c2c-2ed7f11a2f7f.png)

Pe scurt, pentru utlizare, introducem cuvantul pe care il dorim in casuta de cautare si apasam pe butonul SUBMIT, ne sunt prezentate urmatoarele sectiuni "Word, Definition, Example si How to spell?". Daca dorim sa cautam alt cuvant sau acelasi cuvant pentru a vedea o alta interpretare a lui apasam mai intai pe butonul RESET si apoi cautam ce ne dorim. 




