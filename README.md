# Life Saving Seconds
## Predicting Troponin to Fast-Track Heart Attack Treatment

**Disclaimer: Dies ist eine öffentliche Version des Repositorys und enthält nicht die benötigten Datensätze für das Training der Algorithmen!**

Dieses Notebook ist ein Projekt, das von Sejma Sijaric und Fulya Gerin, Bachelor-Studentinnen der Hochschule St. Gallen, entwickelt wurde. Ziel des Projekts ist es, mithilfe von Machine Learning den Troponin-Wert im Blut vorherzusagen. Dieser Wert spielt eine entscheidende Rolle bei der schnellen Diagnose und Behandlung von Herzinfarkten.

Im Rahmen des Projekts wurden Supervised Learning-Modelle trainiert, um den Troponin-Wert basierend auf anderen Blutwerten zu prognostizieren. Das Notebook umfasst die Datenaufbereitung, die Analyse der Feature-Importance und das Training von Regressions- sowie Klassifikationsmodellen.

Das Projekt ist in Python (Version 3.10.7) entwickelt.

## Inhaltsverzeichnis

1. [Installation](#Installation)
2. [Use Case](#Use-Case)
3. [Features](#Analyse-und-Ergebnisse)
4. [Beiträge](#Beiträge)

## Installation 

1. Repository klonen:

   ```bash
   git clone https://github.com/<username>/BachelorProject.git
   cd BachelorProject
2. Abhängigkeiten installieren
    ```
    pip install pandas
    pip install numpy
    pip3 install scikit-learn
    ```    
    Für Scikit-Learn kann auch diese Webseite verwendet werden: https://scikit-learn.org/1.6/install.html
3. Notebook train-test-split.ipynb ausführen, um die benötigten Datensätze zu generieren.  
*Nicht möglich! Datensätze sind nicht verfügbar. 
5. Sobald die Datensätze vorbereitet sind, können die Machine-Learning-Modelle trainiert werden. Viel Spaß!

## Use Case

Das Ziel dieses Projekts ist es, medizinisches Fachpersonal durch präzise Vorhersagen des Troponin-Werts zu unterstützen. Dies kann die Zeit bis zur Diagnosestellung bei einem Verdacht auf Herzinfarkt deutlich verkürzen und dadurch Leben retten.

## Analyse und Ergebnisse

**1. Modellvergleich**

Verschiedene Machine-Learning-Modelle wurden trainiert und verglichen, darunter:

- Klassifikatoren: Gradient Boosting, Random Forest, Decision Tree
- Regressoren: Random Forest, Decision Tree, Bagging Regressor, Linear Regression, Support Vector Machine  

Die besten Ergebnisse erzielte der Random Forest Regressor mit dem niedrigsten absoluten Fehler.

**2. Feature Importance**

Analyse der wichtigsten Features, die den Troponin-Wert beeinflussen.  
Modell-spezifische Analysen sowie die Lasso-Methode identifizierten folgende 10 wichtigsten Features:
- INTER6Messwert (Interleukin 6)
- PROBNPMesswert (B-type natriuretic peptide)
- TRNMesswert
- FEMesswert (Eisenwert)
- QUIMesswert (Thromboplastinzeit)
- GEMesswert
- HDLMesswert (HDL Cholesterin)
- HSTMesswert
- PTTAFMesswert
- ALBMesswert

**3. Datenaufbereitung**

  Umfassende Bereinigung des Datensatzes:
- Entfernen irrelevanter Variablen
- Definieren von Bins
- Imputation fehlender Werte
- Aufteilung in Training- und Testdatensätze

Dies gewährleistet präzisere Modelltrainings und minimiert Verzerrungen.

**4. Ergebniss**

Mit einem durchschnittlichen absoluten Fehler von ±0.6168 ist der Random Forest Regressor das meist geeignete Modell für diesen Zweck.

## Beiträge

Dieses Projekt wurde von den folgenden Personen entwickelt:

- Fulya Gerin  
    Bachelor-Studentin in Computer Science, Universität St. Gallen
- Sejma Sijaric  
    Bachelor-Studentin in Computer Science, Universität St. Gallen
