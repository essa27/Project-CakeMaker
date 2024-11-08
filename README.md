# Project-CakeMaker
Proiectul poartă denumirea “Cake Maker” și este realizat utilizând limbajul de programare C#. 
Aplicaţia simulează un aparat de făcut prăjituri automat cu resurse nelimitate. Rolul lui principal este să 
servească clientul cu prăjitura dorită. Clientul are acces la un meniu principal care îi va oferi anumite 
posibilităţi de selecţie. Principalele clase ale proiectului sunt cele care urmează: 
• Command Panel - Această componentă este interfaţa cu clientul (command line interface). Are ca 
funcționalități: - Afișarea tuturor produselor disponibile pentru cumpărare; - Afișarea produselor din depozit; - Selectarea produsului dorit din meniu și trimiterea sa mai departe către CommandTaker pentru a 
fi preluată comanda; - Posibilitatea de a comanda mai multe produse de același tip. 
• Command Taker - Această componentă onorează comenzile date de client. Funcționalități: - Preia comanda de la CommandPanel. Verifică dacă produsul se află în CarouselOfCakes (mini 
depozit), dacă acesta există, va fi eliminat din depozit şi îi va fi servit clientului. În cazul în care 
nu se află în CarouselOfCakes, acesta îl va interoga pe CakeMaker cerându-i să onoreze 
comanda; - Verifică capacitatea curentă din CarouselOfCakes; - Dacă capacitatea din Carousel este mică, se va trimita o cerere către CakeMaker pentru a face 
atâtea prăjituri câte sunt necesare pentru a umple CarouselOfCakes la maxim. 
• CarouselOfCakes - Acesta este un depozit de prăjituri. Are o capacitate maximă de 12 prăjituri. El 
va accepta doar elemente de tipul Cake. 
• CakeMaker - Este cel care face prăjitura. El realizează o prăjitură într-un interval specificat în 
rețetă. 
• RecipeCake – Reprezintă rețeta de prăjitură, având ca elemente denumirea prăjiturii și timpul de 
prepare al acesteia. 
• Cake – Clasa prin care se specifică numele prăjiturilor.
