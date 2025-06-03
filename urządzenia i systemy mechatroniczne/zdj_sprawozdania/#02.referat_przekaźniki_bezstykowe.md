Temat: Przekaźniki bezstykowe.
Funkcją przekaźników, nie zależnie czy elektromechanicznymi czy bezstykowymi SSR (Solid Stare Ready), jest sterowanie obwodu głównego, wysokonapięciowego, za pomocą sygnału niskonapięciowego. Najbezpieczniejszym sposobem łączenia takich obwodów jest z separacją galwaniczną, co pozwala uniknięcia przepięć w układzie niskonapięciowym, spowodowanych np. zwarciem czy stanami nieustalonymi. Aby zagwarantować separację galwaniczną musi być przerwa pomiędzy obwodami minimum 3mm, aby uniknąć pojawienia się łuku elektrycznego. Podstawą do wyznaczania tej odległości jest oczekiwane napięcie znamionowe izolacji, przekaźnik powinien wytrzymać napięcie rzędu minimum 2,5kV
Separacja galwaniczna - to fizyczne oddzielenie conajmniej dwóch obwodów elektrycznych, uniemożliwiając przepływ prądu elektrycznego pomiędzy tymi obwodami. Energia i informacje mogą być przekazywane pomiędzy tymi obwodami, np za pomocą fototranzystora. 
symbol i zdjęcie fototranzystora: 
![[fototranzystor.png]]
![[fototranzystorz.jpg]]
Działanie fototranzystora: 
W momęcie gdy oświetlimy bazę powstające w tamtym obszarze elektrony dyfundują poprzez złącze kolektorowe zwiększając jego prąd. W tym samym czasie na bazie powstają dziury elektronowe, które nie przechodzą przez barierę potencjału, tworząc nieskompensowany ładunek, który obniża barierę baza-emiter. W stanie nasycenia fototranzystor jest bardziej czuły niż fotodioda.
Zasada działania przekaźników bezstykowych. 
Przekaźniki bezstykowe inaczej półprzewodnikowe, są wytwarzane z półprzewodników, przez co nie posiadają ruchomych części takich jak styki. Przez odpowiednie połączenie półprzewodników, jesteśmy w stanie sterować wysokim napięciem za pomocą niskiego napięcia co pozwala zabezpieczyć operatora przed niebezpiecznym apięciem.

Przykładowe przekaźniki bezstykowe: 
tranzystor: 
![[tranzystor.png]] ![[tranzystorz.png]]
tranzystor bipolarny jest elementem wykonanym z 3 półprzewdników, ustawionych npn lub pnp w odległości nie więcej niz 1μm. Przez taki tranzystor przepływają prądy obu typów, elektronów i dziur, z tąd określenie tranzystor bipolarny.

tranzystor polowy:
![[tranzystorypolowe.png]] ![[tranzystorpolowyz.png]]
![[tranzystor polowy.png]]
tranzystory polowe są sterowane poprzecznym polem elektrycznym, - są to nośniki jednego znaku, dlatego często są nazywane tranzystorami unipolarnymi. Prąd przepływa pomiędzy źródłem (S) i drenem (D) przez obszar półprzewodnikowy nazywany kanałem, w który wnika pole elektryczne napięcia podanego na bramkę (G)

triak: 
![[triak.png]] 
Triak to podgrupa tyrystorów. Triak może przewodzić prąd w obu kierunkach, po podaniu napięcia na bramkę włącza się on i przewodzi prąd. W triaku nie zaobserwujemy zjawiska wydzielanie się ciepła, ponieważ pojawia się ono tylko gdy prąd jest impendowany, a triak jeśli jest włączony przewodzi prąd bez "blokowania" go. Natomiast gdy jest wyłączony całkowicie nie przewodzi prądu. 
Można je znaleść w ściemniaczach do lamp, regulatory prędkości silnika lub w regulatorach mocy wyjściowej w grzejnikach. 
Wadą triaka jest to że może on się samoczynnie włączyć poprezez nagłą zmianę napięcia na jego zaciskach głównych. Zabezpieczeniem przed tego typu zdarzeniami jest podłączenie obwodu RC pomiędzy głównymi zaciskami. 

Diak:
![[diak.png]]
![[diakz.png]]
Diak jest podobny do Triaka, różnicą jest brak wyprowadzonej bramki. Diak jes telementem dwukierunkowym wyzwalającym używanym do sterowania innymi elementami. Diak zaczyna przewodzić przy napięciu przebicia które ma wartość 20V-40V. Po przebiciu napięcie na nim spada do ok. 5V. Wyłączenie diaka następuje w momecie gdy prąd w obwodzie spadnie poniżej prądu podtrzymania. 

tyryator:
![[tyrystor.png]]
Tyrystur jest zbudowany z 2 tranzystorów połączonych w odpowiedni sposób jak na zdjęciu. Umożliwia przepływ prądu tylko w jednym kierunku od anody do katody. Tyrystor umożliwia bardzo dokładne sterowanie przepływem prądu, co czyni go niezastąpionym w energoelektronice czy automatyce przemysłowej. Działanie tyrystora opiera się na dodatnim sprzężeniu zwrotnym co pozwala utrzymać go w stanie przewodzenia nawet gdy zaniknie sygnał sterujący. 








wady zalety:

co ma być:
co to są
symbole
opis
parametry
prosty układ
wady zalety
gdzie się wykożystuje stykowe bezstykowe
bibliografia
tyrystory tranzystory triaki
transoptory !!

https://www.gotronik.pl/ssr-40da-przekaznik-polprzewodnikowy-fotek-p-5302.html
przykład na dane techniczne konkretnego przekaźnika
batland.com.pl
wikipedia.org
Pracownia Elektryczna elementy układów elektronicznych autorzy: Augustyn Chwaleba, Bogdan Moeschke, Marek Pilawski
Elementy i układy elektroniczne część I pod rekacją Stanisława Kuty 
Elementy i układy elektroniczne część II pod rekacją Stanisława Kuty
allegro.pl
piotr-gorecki.pl
symbole.pl
ebmia.pl
