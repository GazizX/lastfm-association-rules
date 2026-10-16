# Association Rule Mining on Last.fm Listening Data

[English](#english) | [Русский](#русский)

## English

A notebook exploring artist co-listening patterns with frequent-itemset mining and association rules. It compares Apriori, FP-Growth, FP-Max, and HMine on user listening histories for the United States, France, and Brazil.

### Notebook

- `lastfm_association_rules.ipynb` — data preparation, frequent itemsets, rule metrics, and visual analysis.

### Input data

The notebook expects a file named `lastfm.csv` in the repository root with at least `user`, `artist`, and `country` columns. The dataset is not included. Add a link to the original dataset and its license before redistributing a copy.

### Experiments

- Convert user listening histories into a user–artist basket matrix
- Compare Apriori, FP-Growth, FP-Max, and HMine
- Generate rules using confidence thresholds
- Inspect support, confidence, lift, and Jaccard similarity
- Compare rule lengths and visualize metric relationships

### Run

```bash
python -m pip install numpy pandas matplotlib seaborn mlxtend jupyter
```

Place `lastfm.csv` beside the notebook, then open `lastfm_association_rules.ipynb` in Jupyter and run the cells from top to bottom.

## Русский

Ноутбук исследует совместное прослушивание исполнителей с помощью поиска частых наборов и ассоциативных правил. Apriori, FP-Growth, FP-Max и HMine сравниваются на историях прослушиваний пользователей из США, Франции и Бразилии.

### Ноутбук

- `lastfm_association_rules.ipynb` — подготовка данных, частые наборы, метрики правил и визуальный анализ.

### Входные данные

Ноутбук ожидает файл `lastfm.csv` в корне репозитория со столбцами как минимум `user`, `artist` и `country`. Сам датасет не включён. Перед распространением его копии добавьте ссылку на исходный набор данных и сведения о лицензии.

### Эксперименты

- Преобразование истории прослушиваний в матрицу пользователь–исполнитель
- Сравнение Apriori, FP-Growth, FP-Max и HMine
- Построение правил с порогами confidence
- Анализ support, confidence, lift и сходства Жаккара
- Сравнение длины правил и визуализация связей между метриками

### Запуск

```bash
python -m pip install numpy pandas matplotlib seaborn mlxtend jupyter
```

Поместите `lastfm.csv` рядом с ноутбуком, откройте `lastfm_association_rules.ipynb` в Jupyter и выполните ячейки по порядку.
