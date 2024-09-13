# linux-os-II - password generator

Her kan du generere dit nye password med både tal, store og små bogstaver samt specialtegn, hvis du ønsker. Længden af dit nye password er også helt op til dig, det skal bare være mindst 6 lang. Hvis du vælger en længde under 6, så vil det genererede password laves til at være 6 lang.

## Installationsvejledning

1. Klon dette repository i din terminal
```python
git clone https://github.com/DetGrey/linux-os-II
```

2. Naviger ind i mappen
```python
cd linux-os-II
```

3. Giv execution rettigheder
```python
chmod +x password_generator
```

4. Kopier password_generator ind i bin mappen
```python
sudo cp password_generator /usr/bin/
```

5. Generer dit nye password
Minimum password længde er 6. Vælger du noget under, så vil dit password output i stedet være 6 karakterer lang.
```python
# Uden specialtegn
password_generator <password length>

# eller med specialtegn
password_generator <password length> -s
```

For at få genereret et password med specialtegn skal du bare tilføje et flag `-s` eller `--special` efter du har specificeret passwordlængden.

## Exempler med længden 12
```python
# Uden speicaltegn
password_generator 12

# Med specialtegn (alternativ 1)
password_generator 12 -s

# Med specialtegn (alternativ 2)
password_generator 12 --special
```

