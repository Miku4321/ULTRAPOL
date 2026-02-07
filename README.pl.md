[![en](https://img.shields.io/badge/lang-en-blue.svg)](https://github.com/jonatasemidio/multilanguage-readme-pattern/blob/master/README.md)
[![pl](https://img.shields.io/badge/lang-pl-red.svg)](https://github.com/jonatasemidio/multilanguage-readme-pattern/blob/master/README.pl.md)

# ULTRAPOL
ULTRAPOL jest nieoficjalną odnogą innego moda do Ultrakilla o nazwie "ULL" (skrót od "Ultrakill Language Library").
Jeśli zainstalowałeś BepInExa oraz ULL, będziesz mógł użyć plików z tego repozytorium, aby grać w Ultrakilla z polskim tekstem i polską czcionką.

Które treści tłumaczy ten mod:
- [x] Tekst (n.p. napisy, interfejs, książki, nazwy wrogów, opisy broni)
- [x] Czcionka (tzn. polskie znaki)
- [ ] Tekstury (n.p. tekst na ścianie)
- [ ] Linie głosowe (tzn. dubbing)

## Na marginesie
- Będę od czasu do czasu wprowadzał zmiany i poprawki do tłumaczenia. Ta wersja nie jest finalna (zważając na to, że niektóre linie tekstu są puste). Oraz, *być może*, przetłumaczę niektóre tekstury.
- Mimo tego, że przetłumaczyliśmy tekst i dodaliśmy polskie znaki do czcionki, nie przetłumaczyłem ani tekstur, ani linii głosowych. Są inne, polskie drużyny, które pracowały nad dubbingiem, lecz nie mam pojęcia czy udało im się dokończyć ich pracę.
- Ultrakill używa czcionki VCR OSD MONO, która nie posiada polskich znaków (diakrytów), a mod ULL nie naprawia tego błędu. W rezultacie, Ultrakill będzie używał brzydkiej czcionki typu "fallback" dla diakrytów. Aby temu zapobiec, będziesz musiał podmienić plik **ullfont.resource** tym, którym podałem w repozytorium (sekcja "Jak zainstalować" poda ci potrzebne instrukcje)
- W chwili pisania tego repozytorium (7 lutego 2026), najnowsza wersja ULL (1.3.1 beta) jest przeznaczona do wersji gry "patch 16d" (inaczej ULTRA_REVAMP). W niedalekiej przyszłości, ma zostać wydana aktualizacja — doda ona ósmą warstwę piekła — która może popsuć ULL.

## Jak zainstalować
1. Znajdź ścieżkę do folderu gry
	- Otwórz Steam
	- Znajdź **ULTRAKILL** w zakładce **Biblioteka**
	- Naciśnij na **ikonkę z trybikiem**
	- Naciśnij **Zarządzaj**
	- Naciśnij **Przeglądaj pliki lokalne**
  
2. Zainstaluj BepInEx (jest to framework dla modów, konieczny do używania ULL)
	- Pobierz [**BepInEx_win_x64_5.4.23.4.zip**](https://github.com/BepInEx/BepInEx/releases/download/v5.4.23.4/BepInEx_win_x64_5.4.23.4.zip) z [BepInEx releases](https://github.com/BepInEx/BepInEx/releases)
	- Przenieś całą zawartość do folderu <ins>**ULTRAKILL**</ins>

3. Zainstaluj ULL (jest to mod tłumaczeniowy, konieczny do załadowania polskiego tekstu w grze)
	- Pobierz [**UltrakULL-1.3.1-Beta.zip**](https://github.com/ClearwaterUK/UltrakULL/releases/download/v1.3.1-beta/UltrakULL-1.3.1-Beta.zip) z [ULL releases](https://github.com/ClearwaterUK/UltrakULL/releases)
	- Z <ins>**pobranego folderu zip**</ins>, przenieś <ins>**config**</ins> i <ins>**plugins**</ins> do folderu <ins>**ULTRAKILL/BepInEx**</ins> (nawet jeśli folder BepInEx już posiada config i plugins)
	- Odpal grę, aby sprawdzić, czy wszystko zostało poprawnie zainstalowane (powinieneś zobaczyć zakładkę **Language** w menu opcji)
	
4. Dodaj polski tekst
	- Otwórz folder: <ins>**ULTRAKILL/BepInEx/config/ultrakull**</ins>
	- Do tego folderu, wstaw plik **pl-PL.json**

5. Dodaj polską czcionkę
	- Otwórz folder: <ins>**ULTRAKILL/BepInEx/plugins/UltrakULL**</ins>
	- W tym folderze, wstaw i podmień plik **ullfont.resource** tym, którym podałem w moim repozytorium

6. Włącz język polski
	- Odpal grę
	- Otwórz **Options**
	- Otwórz **Languages**
	- Wybierz **Polski (Polish)**
	- Teraz będziesz w stanie grać w Ultrakilla z polskim tekstem oraz polską czcionką. Miłej zabawy :]

7. (Krok bonusowy, opcjonalny) Ukryj konsolę BepInEx
	- Otwórz plik <ins>**ULTRAKILL/BepInEx/config/BepInEx.cfg**</ins> w programie do edytowania tekstu
	- Znajdź sekcję **[Logging.Console]**
	- W tej sekcji, zobaczysz parametr **Enabled**. Zmień jego wartość z *true* na *false*
	- Dzięki temu, konsola już nie będzie się pojawiać po każdym włączeniu gry