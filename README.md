# programowanie-w-jezyku-python

## Najważniejsze komendy Git

### Podstawowe
git status - sprawdź stan repozytorium
git log --oneline - historia commitów w skrócie
git log - pełna historia commitów
git diff - sprawdź co się zmieniło

### Pobieranie
git clone https://... - klonowanie repozytorium
git pull - pobierz zmiany ze zdalnego repozytorium
git fetch - pobierz zmiany bez łączenia

### Wysyłanie zmian
git add . - dodaj wszystkie zmiany
git add nazwa_pliku - dodaj konkretny plik
git commit -m "opis" - zapisz zmiany
git push - wyślij do repozytorium
git push --set-upstream origin main - wyślij i ustaw gałąź nadrzędną

### Gałęzie
git branch - lista lokalnych gałęzi
git branch -a - lista wszystkich gałęzi
git checkout main - przełącz na gałąź main
git checkout -b test - utwórz nową gałąź test
git merge test - połącz gałąź test z obecną
git branch -d test - usuń gałąź test
git rebase main - przenieś zmiany na początek gałęzi main

### Cofanie zmian
git restore nazwa_pliku - cofnij zmiany w pliku
git restore . - cofnij wszystkie zmiany
git reset HEAD~1 - cofnij ostatni commit (zachowaj zmiany)
git reset --hard HEAD~1 - cofnij ostatni commit (usuń zmiany)
git revert HEAD - utwórz nowy commit cofający ostatnie zmiany

### Zdalne repozytorium
git remote -v - sprawdź adres zdalnego repozytorium
git remote set-url origin https://... - zmień adres repozytorium
git remote add origin https://... - dodaj zdalne repozytorium

### Schowek (stash)
git stash - schowaj niezapisane zmiany na później
git stash pop - przywróć schowane zmiany
git stash list - lista schowanych zmian

### Tagi
git tag - lista tagów
git tag v1.0 - utwórz tag v1.0
git push origin v1.0 - wyślij tag do repozytorium

### Konfiguracja
git config user.email email@example.com
git config user.name "Imię Nazwisko"
git config core.autocrlf true - napraw problem z LF/CRLF
git config --list - sprawdź całą konfigurację

### Gitignore
echo ".idea/" >> .gitignore - dodaj .idea do gitignore
echo ".venv/" >> .gitignore - dodaj .venv do gitignore
git rm -r --cached .idea - usuń .idea z repozytorium

### Autoryzacja
git clone https://{token}@{link} - klonowanie z tokenem