## Мои pet-проекты, созданные в процессе обучения. Писал только для себя, для получения и закрепления знаний, проверки различных функций, моделей и т.д., поэтому последовательность, логичность действий и качество кода может хромать 
___
### Репозиторий содержит в себе следующие файлы:
- [ed1-regression.ipynb](https://github.com/miglss/pet-projects/blob/main/ed1-regression.ipynb) Задача регрессии, предсказание стоимости автомобилей. 
Что было сделано:
1. Категоризовали признаки с помощью OHE, отнормировали данные с помощью RobustScaler
2. Проверили работу sklearn linear, sgdregress на кросс валидации (KFold вручную и sklearn.cross_val_score)
3. Проверили работу с регуляризацией + подбором параметров через gridsearchCV
4. Выведена корреляционная матрица, проверена работа PCA + результаты на предсказаний на PCA.
5. Проверена svm с разными ядрами + gridsearch
- [ed2-randomforest-gradient-boost-auc-pr.ipynb](https://github.com/miglss/pet-projects/blob/main/ed2-randomforest-gradient-boost-auc-pr.ipynb) Задача бинарной классификации с дисбалансом классов, предсказание типа клиента.
Что было сделано:
1. Предобработка данных
2. Тестирование решающего дерева, подбор гиперпараметров на cv
3. Тестирование случайного леса, подбор гиперпараметров на cv
4. Тестирование LightGBM, подбор гиперпараметров на cv
5. Тестрование SVM
6. Проверка на метриках AUC, F1-score, визуализация ROC, PR, подбор threshold'а (порога)
- [ed3-cnn-reg-techniecs.ipynb](https://github.com/miglss/pet-projects/blob/main/ed3-cnn-reg-techniecs.ipynb) Задача многоклассовой классификации картинок, предсказание типа патологий на растениях.
Что было сделано:
1. Загрузка данных кастомным датасетом, его настройка с различной аугментацией (повороты, эффекты, нормализация картинок) + подсчет mean,std для normalize
2. Написание собственной CNN сети различной конфигурации (добавление некоторых регуляризаторов - dropout, batchnorm, <-- вместе, weight_decay
3. Обучение на CV
4. Вывод графиков, подсчет метрик
- [ed4-advanced-architectures-transfer-learning.ipynb](https://github.com/miglss/pet-projects/blob/main/ed4-advanced-architectures-transfer-learning.ipynb) Что было сделано:
1. Создание архитектуры с простыми skip-connection'ами
2. Создание архитектуры с DenseBlock'ами
3. Создание архитектуры с Inception'ами
4. Fine-tuning AlexNet (без/с заморозкой некоторых слоев)
- [ed5-semantic-segmentation.ipynb](https://github.com/miglss/pet-projects/blob/main/ed5-semantic-segmentation.ipynb) Задача семантической сегментации картинки на 9 классов. Что было сделано:
1. Кастомный датасет для масок+картинок
2. Аугментация
3. Собственная реализация DeconvNet для семантической сегментации
4. Обучение, визуализация результатов, подсчет качества по метрике mIoU
5. Обучение готовой UNet c backbone mobilenet_v2, визуализация результатов, подсчет mIoU
- [ed8-word2vec.ipynb](https://github.com/miglss/pet-projects/blob/main/ed8-word2vec.ipynb) Создание эмбеддингов слов по диалогам из Симпсонов с помощью Word2Vec. Что было сделано:
1. preprocessing текста (токенизация, стоп слова, стемминг и т.д.)
2. Обучены эмбеддинги слов с помощью Gensim Word2Vec
3. Проверка логичности полученных эмбеддингов - просмотр похожих слов, разница некоторых слов, визуализизация пространства эмбеддингов
4. Загрузка предобученных эмбеддингов glove-wiki-gigaword-50, сравнение с полученными
- [gancats.ipynb](https://github.com/miglss/pet-projects/blob/main/gancats.ipynb) Реализован простенький GAN для генерации кошачьих мордочек 64x64
