Praca licencjacka na kierunku matematyka.
Uniwersytet Warszawski
Wydział Matematyki, Informatyki i Mechaniki

Metoda elementów skończonych dla stacjonarnego opływu przeszkody
Autor: Arkadiusz Słowik
Promotor: dr Piotr Krzyżanowski

Zawartość:
problems - gotowe setupy do liczenia modelu stacjonarnego jednokrotnie oraz wielokrotnie dla siatek różnej gęstości;
fem - funkcje liczące elementy fem np. macierz masy, macierz sztywności, macierz dywergencji (poddywergencji), wektor obciążeń, nałożenie warunków brzegowych, wybór funkcji dirichleta, wybór wektora siły, solver, norma euklidesowa;
main - główny notebook: załadowanie bibliotek i notebooków, ustawienia i wywołanie problemów;
mapping - ciąg technologiczny do mapowania izoparametrycznego, poszerzenie siatki ciśnienia do siatki wektora prędkości;
mesh - funkcje do tworzenia siatki: liczenie elementów w obszarze, wyznaczanie wierzchołków pierwotnych, generowanie siatki;
tests - funkcje testujące macierze, funkcje błędu w normach;
visualization - ciąg technologiczny do wizualizacji: wizualizacja węzłów siatki, wizualizacja rozwiązania;

Sposób użycia:
1) Otworzyć main.ipynb.
2) Załadować biblioteki i notebooki.
3) W ustawieniach problemów:
- wykomentować interesujące ustawienie obszaru przepływu lub napisać własne wg opisu funkcji meshgenerator pliku mesh.ipynb,
- zapisać warunki brzegowe przez podanie tablicy dirichlet_fun ( warunek Dirichleta dany funkcją ) i dirichlet_zero ( warunek Dirichleta == 0 ),
- wybrać funkcję przepływu przypisując liczbę z {1,2,3} do zmiennej dirichlet_function_option z pliku fem.ipynb,
- podać wartość lepkości, przeskalować osie, przeskalować wymiary pojedynczego elementu, wybrać wektor sił poprzez podanie liczby z {1,2,3,4,5,6} wg funkcji force_option z pliku fem.ipynb.
4) Uruchomić rozwiązanie pojedynczego problemu lub podać kolejne rosnące przeskalowania wielkości elementu siatki i uruchomić problem dla wielu siatek.