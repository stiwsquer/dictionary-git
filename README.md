#Dictionary GIT
https://medium.com/@saumya.ranjan/how-to-write-a-readme-md-file-markdown-file-20cb7cbcd6f

###Schemat komunikacji

![gitCommunication](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

![gitReferences](https://marklodato.github.io/visual-git-guide/checkout-files.svg)

###Branch i Head

Branch to gałąź która umożliwia tworzenie rówżnych wersji projektu - wskaźnik na dany commit
Head wskazuje nam na Branch.

###Konfiguracja gita

Skonfigurowanie klienta gita - dodanie nazwy użytkownika i email

`git config --global user.name "John Doe"`

`git config --global user.email "johndoe@example.com"`

###Inicjalizacja repozytorium

`git init `

###Status
Wyświetla informacje na temat katalogu projektu

`git status`

###Przekazanie pliku do śledzenia
Dodaje konkretny plik

`git add <nazwa-pliku>`

Dodaje wszystkie pliki

`git add .`

###Przesłanie do lokalnego repozytorium
Z komentarzem bez tytułu

`git commit -m "<Description>"`

Z komentarzem i tytyłem - w oknie, które się pojawi naciskamy ESC i w pierwszej lini od góry piszemy tytuł a w drugiej opis . Potem ESC:x!

`git commit`
###Przesłanie do working directory z local repo konkretnej wersji

Przesłanie commita

`git checkout <version>`

Przesłąnie brancha

`git checkout <branch-name>`

 ###Wyświetlenie informacji o commitach
Wszystko

`git log`

W jednej lini

`git log --oneline`

###Utworzenie nowego brancha
Będzie zawierał to co jest w aktualnym commicie/branchu

`git branch <new-branch-name>`

Będzie zawierał to co jest w podanej wersji commita

`git branch <new-branch-name> <commit-version-name>`

###Usuwanie Brancha

`git branch -d <nazwa-branch-do-usuniecia>`

###Wyszukiwanie commita po komentarzu

`git log --grep="<description>"`

###Cofanie commita

Cofanie commita przy czym praca w working directory oraz w staging area zostaje 
`git reset --soft`  

Cofanie commita przy czym praca w working directory zostaje ale w staging area nie
`git reset` lub `git reset --mixed` to jest to samo

Cofanie commita i usuwanie pracy nawet z working directory - całkowicie usuwa dane

`git reset --hard`

###Scalanie różnych wersji projektu

Gdy np. jesteśmy na branch master to jeśli użyjemy komendy merge to branch master nam się zmieni (zaaktualizuje)

`git merge <nazw-brancha-z-którym-chcemy-zmergować`

###Odkładanie elementów na stos

`git stash` lub `git stash push -m "<description>"`

###Wypisanie elementó znajdujących się na stosie

`git stash list`

###Pobranie pierwszego elementu ze stosu

`git stash pop`


###Pobranie dowolnego elementu ze stosu

`git stash pop stash@{<index>}`


###Czyszczenie stosu

`git stash clear`

