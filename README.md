# CardioML
Data Intensive Project on Cardiotocographic data

## Modelli da fare

### MOdelli per regressione
- Regressione Lineare (sarà una merda) `LinearRegression()`
    - Feature Polinomiali `PolynomialFeatures(degree=x)`
    - Standardizzazione dei dati (`StandardScaler`, `MinMaxScaler`)

- Regressione non Lineare (sempre con `PolynomialFeatures`, e poi aggiungere
linear regression con le funzioni kernel o con func di regolarizzazione).
    - Regolarizzazione (`Ridge`, `Lasso`, `ElasticNet`)

    - Funzioni Kernel ('regr': `KernelRidge`) con kernel:
        - `poly` a vari gradi (range(1, 5) magari)
        - `rbf` a vari valori di `gamma`
        - quando si usa `KernelRidge`, non usare `PolynomialFeatures`.
    - Cross validation per ogni modello (k=3 fold con shuffle)
    - Ricerca best iperparametri con grid search
        - Più che usare solo la grid search, usare anche la funzione cross validate
          per ottenere statistiche sulle varie misurazione (vedi lab07).

### Modelli per classificazione
