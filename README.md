#Zadanie 7

import random

cena = 6.5
droga = random.randint(1, 1000)
spalanie = float(input("ile pali twoj samochod [l/100km]: "))
benzyna = droga/100 * spalanie
koszty = benzyna * cena
print(f"W trakcie przejechanej trasy w {droga}km twoj samochod spali {benzyna} litrow paliwa, co bedzie ci kosztowalo {koszty} zlotych"

#Zadanie 16

import math


a = int(input("Podaj długosc pierwszego boku: "))
b = int(input("Podaj długosc drugiego boku: "))
c = int(input("Podaj długosc trzeciego boku: "))

obw = 2 * a + 2 * b + 2 * c

print(f"Oto jest obwód prostokątą: {obw}")

p = (a + b + c)/2
pole = sqrt = math.sqrt(p*(p - a)*(p - b)*(p - c))


#nie wiem czy potrzebna jest liczba całkowita, dlatego nic nie zmienialem poniżej
print("Oto jest pole prostokątą: " + str(pole))



#Zadanie 17

letter = input("Wprowadź jedną literę: ")

if len(letter) == 1 and letter.isalpha():
	asci = ord(letter)
	if 65 <= asci <= 90:
		print("Wprowadzana litera jest dużą literą")
	elif 97 <= asci <= 122:
		print("Wprowadzona litera jest małą literą")
else:
	print("Wprowadzono błąd")

#Zadanie 19

def con(char):
	asci = ord(char)
	if 'A' <= char <= 'Z':
		return chr(asci + 32)
	elif 'a' <= char <= 'z':
		return chr(asci - 32)
	else:
		return char
literka = input("Proszę o podanie litery: ")
if len(literka) == 1:
	print("Proszę bardzo:", con(literka))
else:
	print("Wprowadź tylko jedną literę.")

 #Zadanie 20
 
 def obl_wynik(gol, bonus):
	wynik = gol * 10
	if gol > 5:
		wynik += 5
	elif gol > 10:
		wynik += 10
	wynik += bonus

	return wynik
try:
	gol = int(input("Wprowadź liczbę bramek zdobytych przez drużynę: "))
	bonus = int(input("Wprowadź liczbę bonusów zdobytych przez drużynę: "))

	wyn_druzyny = obl_wynik(gol, bonus)

	print("Łączny wynik drużyny:", wyn_druzyny)

except ValueError:
	print("Proszę wprowadzić poprawne liczby całkowite.")





























