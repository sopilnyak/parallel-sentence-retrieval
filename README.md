# Извлечение параллельных предложений из сравнимых корпусов

Здесь находится исходный код экспериментов по извлечению параллельных предложений в рамках магистерской диссертации и полученные в результате корпуса.

## Корпуса

* TTW (Tatoeba, TED 2013, WMT-News) | [en](https://drive.google.com/file/d/1dcCfUNuWmqHmcZgg00JB-GkapulTKDYx/view) | [ru](https://drive.google.com/file/d/1Jhy4xHWSqmF9yxM5-SzeNpUhwpaMJSDh/view) | [gold](https://drive.google.com/file/d/1_Hqu9_0KB1DR40wXZu0yg4xFRNdYJ1ym/view)
* Wikipedia (10000 статей из Википедии) | [en](https://drive.google.com/file/d/1c_zwbY4v9zgqxwUiRkiWW76PQWo-9fg7/view) | [ru](https://drive.google.com/file/d/1YBzxcUzbhFZib9Xj3UKlude9maTuKeJu/view) | [извлеченные параллельные предложения](https://drive.google.com/file/d/1-04sFmP-Bn96Mj8iZe2tBSXeG20dAa05/view)
* COVID (новости с 12 по 19 апреля 2020) | [en](https://drive.google.com/file/d/1-Sn-7jLrmMXfA3O0TQRQmYJw-PIt_1Ww/view) | [ru](https://drive.google.com/file/d/1-9hbcjcDNrEpFhfawEPNFlU05v0cf5ZG/view) | [извлеченные параллельные предложения](https://drive.google.com/file/d/1NxSCW3uOQLxTzWkAgGBit23ZwG62Uo4h/view)

## Эксперименты

* [Получение](https://github.com/sopilnyak/parallel-sentence-retrieval/xlm_r_experiments.ipynb) эмбеддингов из предобученной межъязыковой модели [XLM-R](https://github.com/facebookresearch/XLM) и обучение слоев поверх нее
* [Формирование](https://github.com/sopilnyak/parallel-sentence-retrieval/data_for_training.ipynb) датасета для обучения классификатора и эмбеддингов
* [Составление](https://github.com/sopilnyak/parallel-sentence-retrieval/ttw_mining.ipynb) корпуса TTW на основе параллельных корпусов
* [Составление](https://github.com/sopilnyak/parallel-sentence-retrieval/scraping.ipynb) корпусов Wikipedia (10000 статей из Википедии) и COVID (новости с 12 по 19 апреля 2020)

## Зависимости

* Python 3.6
* [PyTorch 1.5](https://pytorch.org/)  
* [transformers](https://github.com/huggingface/transformers) (работа с предобученными языковыми моделями)  
* [faiss](https://github.com/facebookresearch/faiss) (поиск ближайших векторов на GPU)  
* [laser_wrapper](https://github.com/sopilnyak/laser_wrapper) (обертка над эмбеддингами [LASER](https://github.com/facebookresearch/LASER))  
* [DeepPavlov](https://github.com/deepmipt/DeepPavlov) (сегментатор)  
* [newspaper3k](https://github.com/codelucas/newspaper) (scraping новостных статей)
