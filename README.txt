Добрый день! 

Ноутбуки eda_and_data_prep, xgb_model и stacking выполнялись с помощью Google Colab Pro (L4 GPU и 52gb ОЗУ)

Ноутбуки catboost_model и lgbm_model выполнялись локально (RTX 4070s GPU и 64gb ОЗУ)

Рекомендуемая последовательность запуска файлов: 

1. eda_and_data_prep (исследователький анализ данных и предобработка)
2. catboost_model (построение модели catboost)
3. lgbm_model (построение модели lgbm)
4. xgb_model (построение модели xgboost)
5. stacking  (стэкинг трех моделей)

Также в папке artifacts находятся: 
файлы предсказаний моделей на обучающей выборке для стекинга:

1. catboost_86.11_train_preds
2. lgbm_85.9_train_preds
3. xgb_85.99_train_preds

файлы предсказаний моделей на тесте (сабмиты):

1. catboost_86.11_test_preds
2. lgbm_85.9_test_preds
3. xgb_85.99_test_preds

а также информация о важности фичей по шап для моделей catboost и lgbm:

1. catbost_feature_imp 
2. lgbm_feature_imp

и файл train_targets, который содержит таргеты трейна (нужны для обучения мета модели)

Если возникнут вопросы, с радостью ответим в телеграмме: @taychinov @Doppler67




