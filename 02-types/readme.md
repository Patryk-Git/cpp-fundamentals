**void - typ pusty**

*   Używaj tylko, by zaznaczyć, be funkcja nic nie zwraca.
*   Nie modna tworzyć obiektów typu waid.
*   Nie uływaj wakadników void" to zła praktyka w C++.

**bool - typ logiczny**

*   Ma diviemodliwe wartośck true albo false.
*   `sizeof(bool)` `1` `[B]` (zazwyczaj równy)

**char - typ znakowy**

*   Służą do przechowywania pojedynczych znaków ASCII, które pod spodem są reprezentowane jako liczba.
*  `sizeof(char)` `1` `[B]`
*   `char` - przechowuje wartości od -128 do 127
*   `unsigned char` - przechowuje warto od 0 do 255
*  `unsigned` oznacza, że typ zmiennej jest bez znaku (nie przechowuje wartości ujemnych)

**Typy całkowitoliczbowe**

*   Służą jak nazwa wskazuje do zapisania liczb całkowitych (bez części ułamkowej). Mają ograniczony rozmiar.
    *   `short` / `unsigned short` - rozmiar => `2` `[B]`
    *  `int` / `unsigned int` - rozmiar => `2` `[B]`
    *  `long` / `unsigned long` - rozmiar => `4` `[B]`
    *  `long long` / `unsigned long long` - rozmiar => `8` `[B]`

**Typy zmiennoprzecinkowe**
*   Służą do przechowywania liczb, które posiadają część ułamkową lub niesamowicie duże. Łatwiej myśleć tutaj o liczbach w notacji wykładniczej, np. 3.54E-14, 6.2222234
*   Szczegóły reprezentacji liczb zmiennoprzecinkowych i operacji na nich w systemie binarnym podaje standard IEEE754. Jeśli chcesz wiedzieć więcej o IEEE754, obejrzyj to video
    * `float` - rozmiar: zwykle `4` `[B]`
    * `double` - rozmiar: zwykle `8` `[B]`
    * `long double` - rozmiar: zwykle `10` `[B]`
    * Zawsze mogą mieć wartości ujemne (brak wersji `unsigned`)
    * Posiadają specjalne wartości:
        * `0.0` (-ujemne zero)
        * `-Inf` (-nieskończoność)
        * `NaN` (Not a Number) - dana liczba nie jest poprawna.
*   UWAGA! Nie porównuj operatorem `==` liczb zmiennoprzecinkowych (z powodu utraty precyzji możesz dostać błędne wyniki)
*   UWAGA! Porównanie `NaN == NaN` daje `false`