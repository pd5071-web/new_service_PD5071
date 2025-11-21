# Projekt: Dokumentacja rozwoju usługi medycznej AR‑Rehab

## 1. Opis usługi medycznej

AR‑Rehab to usługa medyczna wykorzystująca technologię rozszerzonej
rzeczywistości (AR) do prowadzenia rehabilitacji w warunkach domowych.
System pozwala pacjentom wykonywać ćwiczenia z wirtualnymi instrukcjami,
analizuje poprawność ruchów w czasie rzeczywistym oraz dostosowuje
program terapii do postępów użytkownika.

Pełny opis znajduje się w pliku **opis_usługi.txt**.

## 2. Dokumenty stworzone w projekcie

W repozytorium znajdują się następujące pliki dokumentacyjne:

### • opis_usługi.txt

Szczegółowy opis usługi AR‑Rehab, jej celu, grupy docelowej oraz
korzyści dla pacjentów.

### • plan_wdrożenia.txt

Plan wdrożenia usługi wraz z datami i kolejnymi etapami.

### • ryzyka.txt

Lista potencjalnych ryzyk związanych z korzystaniem z usługi opartej na
AR.

### • kampania_marketingowa.txt

Plan kampanii informacyjno‑marketingowej promującej usługę AR‑Rehab.

### • ankieta_pacjentów.txt

Ankieta przygotowana z myślą o zebraniu opinii pacjentów dotyczących
usługi.

### • images/

Folder zawierający logo usługi AR‑Rehab (plik binarny dodany zgodnie z
poleceniem).

### • moje_notatki.txt

Plik utworzony zgodnie z instrukcją --- **nie jest śledzony przez GIT**,
ponieważ znajduje się w pliku `.gitignore`.

## 3. Instrukcje dotyczące pracy z repozytorium

### Pobranie repozytorium

    git clone https://github.com/<twoje_konto>/new_service_PD5071.git
    cd new_service_PD5071

### Praca z gałęziami

Wyświetlenie gałęzi:

    git branch

Stworzenie nowej gałęzi marketing:

    git checkout -b marketing

Przełączenie gałęzi:

    git checkout main

Scalanie gałęzi marketing z główną:

    git merge marketing

### Przywracanie wcześniejszych wersji dokumentów

Wyświetlenie historii:

    git log

Przywracanie pliku:

    git checkout <ID_commit> -- <plik>

## 4. Wykorzystane polecenia Git i ich zastosowanie

-   `git init` --- utworzenie repozytorium\
-   `git add .` --- dodanie plików do śledzenia\
-   `git commit -m ""` --- zapis zmian\
-   `git checkout -b marketing` --- utworzenie gałęzi\
-   `git merge marketing` --- scalanie gałęzi marketing\
-   `git tag v1.0` --- oznaczenie gotowej wersji\
-   `git push` --- wysyłanie zmian do GitHub\
-   `echo "moje_notatki.txt" >> .gitignore` --- wpisanie pliku do
    ignorowania\
-   `git add .gitignore` --- dodanie konfiguracji ignorowania

## 5. Opis napotkanych problemów i sposoby ich rozwiązania

### Problem 1: Błąd uwierzytelnienia GitHub (403)

Terminal odrzucał token przy próbie `git push`.

**Rozwiązanie:**\
Utworzenie nowego *fine‑grained token*, ustawienie „Contents: Read and
Write", usunięcie starych wpisów z Keychain.

### Problem 2: Terminal nie wyświetlał wpisywanego tokenu

Wpisywanie wyglądało jak zawieszone okno.

**Rozwiązanie:**\
Token należy wkleić mimo braku reakcji --- terminal celowo ukrywa wpis.

### Problem 3: Wątpliwości przy scalaniu gałęzi marketing

Scalanie odbyło się bez konfliktów:

    git checkout main
    git merge marketing

## 6. Wersja końcowa projektu

Gotowa wersja projektu została oznaczona tagiem:

    v1.0 – Gotowy plan wdrożenia usługi medycznej


------------------------------------------------------------------------

Dokument przygotowany zgodnie z wymaganiami projektu końcowego System Kontroli
Wersji.
