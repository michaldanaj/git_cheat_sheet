## Komendy

* add files - przenosi wybrane pliki do stege'a, śledzi je

* branch - zarządzanie gałęziami
  ```
  branch - wyświetla gałęzie w repozytorium
  ```

* checkout - przywraca dany stan
  ```
  checkout -- plik - usuwa zmiany, które nie zostały jeszcze przeniesione do stage'a (przywraca stage)
  checkout hash plik - przywraca plik z commita o danym hash - zapisane to jest jak kolejny commit
  checkout branch - zmienia gałąź  (przywraca stan danej gałęzi)
  checkout -b branch - tworzy nową gałąź o nazwie branch z aktywnej gałęzi
  ```

* commit - zapisuje zmiany które są stage'u
  ```
  commit - otwiera edytor aby wpisać komentarz i commituje
  commit -m "tekst" - robi commit z komentarzem (message)
  ```
  
* config - konfiguracja
  ```
  config --list --system - wypisuje ustawienia dla każdego użytkownika
  config --list --global - wypisuje ustawienia ddla każdego projektu użytkownika
  config --list --local - wypisuje ustawienia ddla danego projektu
  config --global setting.name setting.value - ustawia konfigurację 
  config --global user.name setting.value - ustawia usera 
  config --global user.email setting.value - ustawia jego email
  ```

* diff - pokazuje różnice
  ```
  git diff - 
  git diff id1..id2 - różnice między rewizjami z hash = id1 i hash = id2
  git diff branch1..branchd2 - różnice między gałęziami
  ```
  

* log - pokazuje zmiany w repozytorium
  ```
  log - wszystkie zmiany
  log plik - zmiany danego pliku
  ```
  
* merge - łączy gałęzie
  ```
  merge source destination - nie jestem pewny, że taka kolejność. Może dlaego, że robiłem merge z konfliktem. Zrobił merga do 
     aktywnej gałęzi którą była source.
  ```
  
* reset - przywraca stan sprzed zmian które są już w stage'u (usuwa to co jest w stage) i przywraca daną rewizję
  ```
  git reset HEAD filename
  ```
  
* rm - usuwa plik. Na pewno z katalogu roboczego. I chyba od razu tą zmianę wrzuca do stage'a


* show - opis commita wzkazanego bezwzględnie (hash) albo względnie
  ```
  show 41AFD323
  show HEAD~2
  ```
  
* annotate file - wypisuje kto i kiedy zmienił daną linię w pliku
  
* clean - usuwa nieśledzone pliki
  ```
  clean -n - pokazuje listę nieśledzonych plików (potencjalnie do usunięcia)
  clean -f - usuwa pliki
  ```


## Ścieżka względna zmian
* HEAD - najświeższy commit
* HEAD~n - commit n przed HEAD
