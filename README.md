# what_what


## Jak uruchomić:

Będąc na przygotowanym serwerze albo u siebie na przygotowanym komputerze (przygotowanym czyli masz git, python3, pip3, venv, ssh).

#### Pobierz:

```
cd /var/www
git clone https://github.com/ZPXD/what_what.git/
```

#### Uruchom środowisko:

```
python3 -m venv flagaenv
source flagaenv/bin/activate
```

#### Zainstaluj wymagane biblioteki:
```
pip3 install -r requirements.txt
```

#### Uruchom program:

```
export FLASK_APP=app.py
flask run
```

#### Oglądaj rezultaty w przeglądarce

#### A: na własnym kompie:

Po odpaleniu aplikacji wejdź na http://127.0.0.1:5000/

#### B: na serwerze:

Otwórz nowy terminal lub powershell będąc na swoim komputerze i wpisz:

za username -  wstaw nazwę użytkownika
za nazwa_klucza - nazwę klucza
za 1.1.1.1 – ip serwera
```
ssh -L 5000:localhost:80 -i nazwa_klucza username@1.1.1.1
```

I wejdź na http://127.0.0.1:5000/


##Windows:

U siebie na kompie potrzebujesz git, Git Bash, python, pip, venv, ssh)

###Utwórz nowy folder do projektu i pobierz:

```
mkdir whatwhat
cd whatwhat
git clone https://github.com/ZPXD/what_what.git/
```
#### Utwórz i uruchom środowisko:
```
py -3 -m venv flagaenv
flagaenv\Scripts\activate
```

#### Zainstaluj wymagane biblioteki:
```
cd what_what
pip install -r requirements.txt
```

#### Uruchom program:

```
$env:FLASK_APP = "app" #nie trzeba jeśli aplikacja nazywa sie app.py
flask run
```

### Uruchom program w trybie debugowania:

```
$env:FLASK_ENV = "development"
flask run
```
wejdź na http://127.0.0.1:5000/
