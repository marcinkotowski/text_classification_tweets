
# Klasyfikacja emocji na podstawie tweetów

## Opis Projektu

Projekt ten obejmuje analizę sentymentu na danych z Twittera. Wykorzystano różne modele, takie jak Regresja Logistyczna, Maszyna Wektorów Nośnych (SVM), Las Losowy (RF), oraz Konwolucyjna Sieć Neuronowa (CNN) z osadzeniem słów.

## Instrukcje Użycia

1. Pobierz repozytorium lokalnie:

   ```bash
   git clone https://github.com/marcinkotowski/text_classification_tweets
## Wyniki Modeli
Oczywiście, przepraszam za zamieszanie. Oto analiza i recenzja wyników modeli w języku polskim:

### Model 1: Regresja Logistyczna (LR) z WordLevel TF-IDF
- **Precyzja:** 0,8072
- **Czułość:** 0,7973
- **Wskaźnik F1:** 0,8023
- **Dokładność:** 0,7654

### Model 2: Maszyna Wektorów Nośnych (SVM) z wektorami N-Gram
- **Precyzja:** 0,9265
- **Czułość:** 0,9314
- **Wskaźnik F1:** 0,9289
- **Dokładność:** 0,9159

### Model 3: Las Losowy (RF) z WordLevel TF-IDF
- **Precyzja:** 0,9188
- **Czułość:** 0,9179
- **Wskaźnik F1:** 0,9183
- **Dokładność:** 0,9056

### Model 4: Konwolucyjna Sieć Neuronowa (CNN) z osadzeniem słów
- **Precyzja:** 1,0
- **Czułość:** 0,3641
- **Wskaźnik F1:** 0,5338
- **Dokładność:** 0,3641

## Analiza:

1. **Regresja Logistyczna (LR):**
   - Porządna precyzja, czułość i wskaźnik F1.
   - Dokładność jest niższa w porównaniu do SVM i RF.

2. **Maszyna Wektorów Nośnych (SVM):**
   - Wysoka precyzja, czułość i wskaźnik F1.
   - Doskonała dokładność, lepsza niż w przypadku LR.

3. **Las Losowy (RF):**
   - Dobra precyzja, czułość i wskaźnik F1.
   - Dokładność jest nieco niższa niż w SVM, ale wciąż solidna.

4. **Konwolucyjna Sieć Neuronowa (CNN):**
   - Perfekcyjna precyzja sugeruje, że model poprawnie przewiduje wszystkie istotne przypadki.
   - Niska czułość wskazuje, że model pomija wiele istotnych przypadków.
   - Niski wskaźnik F1 sugeruje kompromis między precyzją a czułością.
   - Dokładność jest najniższa spośród wszystkich modeli.

## Wnioski:
- **SVM i RF** radzą sobie dobrze pod względem precyzji, czułości i dokładności.
- **CNN** osiąga perfekcyjną precyzję, ale kosztem niskiej czułości, co sugeruje, że model ma tendencję do klasyfikowania większości przypadków jako nieważne.
- Wybór najlepszego modelu zależy od konkretnych wymagań aplikacji. Jeśli istotna jest wysoka czułość, preferowany może być SVM.
