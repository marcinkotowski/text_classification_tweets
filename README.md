
# Klasyfikacja emocji na podstawie tweetów

## Opis Projektu

Projekt ten obejmuje analizę sentymentu na danych z Twittera. Wykorzystano różne modele, takie jak Regresja Logistyczna, Maszyna Wektorów Nośnych (SVM), Las Losowy (RF), oraz Konwolucyjna Sieć Neuronowa (CNN) z osadzeniem słów.

## Instrukcje Użycia

1. Pobierz repozytorium lokalnie:

   ```bash
   git clone https://github.com/marcinkotowski/text_classification_tweets
## Wyniki Modeli

### Model 1: LR, WordLevel TF-IDF
- **Precision:** 0.8119
- **Recall:** 0.7627
- **F1 Score:** 0.7865
- **Accuracy:** 0.7446

### Model 2: SVM, N-Gram Vectors
- **Precision:** 0.9215
- **Recall:** 0.9280
- **F1 Score:** 0.9248
- **Accuracy:** 0.9133

### Model 3: RF, WordLevel TF-IDF
- **Precision:** 0.9123
- **Recall:** 0.9181
- **F1 Score:** 0.9152
- **Accuracy:** 0.9047

### Model 4: CNN, Word Embeddings
- **Precision:** 1.0
- **Recall:** 0.3626
- **F1 Score:** 0.5322
- **Accuracy:** 0.3626
- 
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
