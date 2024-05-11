# Описание финального проекта

Cоздание семантической системы маркировки ролей с использованием моделей обучения машин СОТА

## Авторы

- [Сударчиков Глеб]: подход Maxent Baseline
- [Дубенец Владислав]: Метод случайного леса
- [Горбунов Андрей]: Надежно оптимизированный подход BERT
- [Краснов Андрей]: подход BERT - базовая модель

## Эксперементы

- Baseline: [Maxent](https://github.com/dizys/nyu-nlp-homework-6)
- Random Forest: [Notebook](./src/RandomForest.ipynb)
- BERT (base): [Notebook](./src/bert_based.ipynb)
- RoBERTA: [Notebook](./src/hf_transformer_roberta.ipynb)

## Результаты

On %-test:

| Model                     | Precision | Recall |    F1     | Output                                              |
| :------------------------ | :-------: | :----: | :-------: | :-------------------------------------------------- |
| Maxent                    |   71.88   | 61.33  |   66.19   | [txt](./out/%-out/test-out-maxent.txt)              |
| RandomForest              |   64.53   | 74.00  |   68.94   | [txt](./out/%-out/test-out-rf.txt)                  |
| BERT                      |   91.33   | 91.33  |   91.33   | [txt](./out/%-out/test-out-bert.txt)                |
| DistilBERT                |   93.75   | 90.00  |   91.84   | [txt](./out/%-out/test-out-distilbert.txt)          |
| RoBERTA                   |   91.50   | 93.33  |   92.41   | [txt](./out/%-out/test-out-RoBERTA.txt)             |

On total-test:

| Model      | Precision | Recall |  F1   | Output                                         |
| :--------- | :-------: | :----: | :---: | :--------------------------------------------- |
| Maxent     |   55.33   | 36.02  | 43.64 | [txt](./out/total-out/test-out-maxent.txt)     |
| DistilBERT |   80.49   | 78.43  | 79.45 | [txt](./out/total-out/test-out-distilbert.txt) |
