# Predviđanje potrošnje kalorija (Calorie Expenditure Prediction)

## Opis projekta

Ovaj projekat se bavi predviđanjem potrošnje kalorija korišćenjem algoritama mašinskog učenja.

Cilj projekta je analiza podataka o fizičkoj aktivnosti i izgradnja regresionih modela koji na osnovu dostupnih karakteristika predviđaju broj potrošenih kalorija.

Projekat je izrađen u okviru fakultetskih obaveza, sa fokusom na obradu podataka, vizualizaciju, treniranje modela i procenu njihovih performansi.

## Korišćene tehnologije

- **Python** – programski jezik
- **pandas i NumPy** – obrada i analiza podataka
- **Matplotlib i Seaborn** – vizualizacija podataka
- **scikit-learn** – implementacija i evaluacija modela mašinskog učenja
- **Jupyter Notebook** – razvoj i dokumentovanje analize

## Modeli mašinskog učenja

U projektu su implementirana i upoređena dva regresiona modela:

### Linear Regression

Linearni regresioni model koji predviđa potrošnju kalorija na osnovu linearnih odnosa između ulaznih karakteristika i ciljne promenljive.

### Random Forest Regressor

Ansambl algoritam koji koristi više stabala odlučivanja kako bi modelovao složenije odnose između podataka i predvideo potrošnju kalorija.

## Tok rada

1. Učitavanje i pregled skupa podataka.
2. Eksplorativna analiza i vizualizacija podataka.
3. Priprema ulaznih karakteristika i ciljne promenljive.
4. Podela podataka na trening i test skup.
5. Standardizacija ulaznih karakteristika.
6. Treniranje modela Linear Regression i Random Forest.
7. Evaluacija i poređenje rezultata korišćenjem metrika MAE, MSE i R².

## Evaluacija modela

Za procenu performansi korišćene su sledeće metrike:

- **MAE (Mean Absolute Error)** – prosečna apsolutna greška predviđanja.
- **MSE (Mean Squared Error)** – prosečna kvadratna greška predviđanja.
- **R² (Coefficient of Determination)** – pokazuje koliko dobro model objašnjava varijabilnost ciljne promenljive.

### Rezultati modela

| Model | MAE | R² |
|---|---:|---:|
| Linear Regression | 8,44 | 0,97 |
| Random Forest Regressor | 1,72 | ≈ 1,00 |

*Prikazane su zaokružene vrednosti rezultata na test skupu.*

Na osnovu dobijenih rezultata, **Random Forest Regressor ostvaruje bolje performanse** od modela Linear Regression.

Random Forest ima manju prosečnu apsolutnu grešku, što ukazuje na preciznija predviđanja potrošnje kalorija na korišćenom test skupu. Oba modela postižu visoke vrednosti R², ali Random Forest bolje modeluje odnose između ulaznih karakteristika i ciljne promenljive.

## Pokretanje projekta

1. Preuzeti ili klonirati repozitorijum.
2. Instalirati potrebne biblioteke pomoću komande:

   `pip install -r requirements.txt`

3. Otvoriti `calorie_prediction.ipynb` u Jupyter Notebook-u ili VS Code-u.
4. Proveriti da se `calories.csv` nalazi u folderu projekta.
5. Pokrenuti sve ćelije redom.

## Zaključak

Projekat prikazuje primenu tehnika mašinskog učenja za rešavanje regresionog problema, uključujući analizu i pripremu podataka, treniranje različitih modela i poređenje njihovih performansi.

Na osnovu evaluacije, Random Forest Regressor pokazao se kao uspešniji model za predviđanje potrošnje kalorija na korišćenom skupu podataka.

Projekat predstavlja praktičnu primenu Python biblioteka za analizu podataka, vizualizaciju i mašinsko učenje.

## Izvor podataka

Za izradu projekta korišćen je javno dostupan skup podataka **Calories Burnt Prediction**, objavljen na platformi Kaggle.

- **Autor:** Ruchika Kumbhar
- **Izvor:** https://www.kaggle.com/datasets/ruchikakumbhar/calories-burnt-prediction

Podaci su korišćeni za akademsku analizu, treniranje i evaluaciju regresionih modela.