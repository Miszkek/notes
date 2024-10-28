# Podstawowe Parametry Układów Cyfrowych

1. Do podstawowych parametrów półprzewodnikowych scalonych układów cywfrowych należą:

***- Czas propagacji - $t_p$, określający szybkość działania układu.
- Straty mocy - (moc pobierana), moc rozpraszana), określające moc pobieraną z zasilacza.
- Margines zakłóceń $\delta$U określający odporność układu na zakłucenia.***

Wartości typowe tych parametrów są najczęściej wykorzystywane do analizy porównawczej serii układów wykonanych w różnych technologiach, przez różnych producentów. Parametry te mogą być przydatne użytkownikowi przy wyborze serii układów.

Projektanta systemów cyfrowych interesują takie parametry jak:
- napięcia
- prądy zasilania
- napięcia i prądy wejściowe/wyjściowe, obciążalność wyjść asortyment układowy i inne.

Znajomość tych wszystkich parametrów umożliwia świadomy i optymalny wybór określonej klasy układów do konkretnych zastosowań, a także właściwą ich eksploatację.
Na oznaczenie poszczególnych parametrów przyjęto używać pewne symbole literowe, których znaczenie staje się oczywiste, jeśli jest znane ich pochodzenie.

2. Jak większość tego typu określeń i symboli (stosowanych w technice cyfrowej), tak i te mają swoje źródło w języku angielskim.
Litera:
- **I** pochodzi od angielskiego słowa ***Input*** - wejście, litera
- **O** pochodzi od ***Output*** - wyjście
- **H** od **High** - wysoki
- **L** od **Low** - niski
- **S** od **Shorting (Shoirt-circut)** - zwarcie
- **P** od **Propagation** - propagacja

Uwzględniając powyższe uwagi znacznie niżej podanych symboli staję się oczywiste i łatwiejsze do zapamiętania.

3. **Parametry Statyczne**

- $U_{CC}$ - napięcie zasilania
- $U_{IH}$ - napięcie wejściowe w stanie wysokim
- $U_{IL}$ - napięcie wejściowe w stanie niskim 
- $U_{OH}$ - napięcie wejściowe w stanie wysokim
- $U_{OL}$ - napięcie wejściowe w stanie niskim

- $I_{IH}$ - prąd wejściowy w stanie wysokim
- $I_{IL}$ - prąd wejściowy w stanie niskim 
- $I_{OH}$ - prąd wyjściowy w stanie wysokim
- $I_{OL}$ - prąd wyjściowy w stanie niskim
- $I_{CCH}$- prąd wejściowy w stanie 
- $I_{CCL}$- prąd wejściowy w stanie 
- $I_{OS}$ - wyjściowy  zwarciowy

- $\delta U_L$ - margines zakłóceń w stanie niskim 
- $\delta U_H$ - margines zakłóceń w stanie wysokim

3. Opuźnienia sygnałów wyjściowych, w stosunku do sygnałów wejściowych, są konsekwencją określonego czasu trwania procesu przełączania, czas ten jest sumą czasu przeładowania pojemności pasożytniczych i czasu przejścia tranzystora ze stanu przewodzenia do stan blokowania. W opóźnieniu pojawionym się w pojawia się jako czas propagacji ***$t_t$***.

Czas propagacji jest istotnym parametrem, dla projektanta i użytkownika systemów cyfrowych, wynika z niego minimalny czas trwania impulsu wejściowego, który spowoduje odpowiedź układu. Impulsy wejściowe o czasie trwania krótszym od czasu propagacji nie zostaną przez układ zauważone.

Zamiast parametru **$t_t$**, można niekiedy mówić o częstotliwości maksymalnej **$f_{max}$**

DATA: 10.10.2024

Układy ***TTL***:
- Operowane napięcie: $+5V +- 5%$
- Odczyt jedynki logczinej: 2.7V - 5V
- Odczyt zera logczinego: 0 - 2.7V


Układy ***CMOS***:
- Operowane napięcie: $+5V - 20V$

- Odczyt jedynki logczinej: 
    4.95V - 5V
    3.5 V - 5V

- Odczyt zera logczinego:
    0 - 0.05
    0 - 1.5V
