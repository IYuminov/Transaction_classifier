# Transaction_classifier
Binary classification of transactions

В данных собрана обезличеная информация о совершенных клиентом транзакциях. Дополнительно собраны сведения о mcc кодах категорий товаров и типе транзакции. Целью было, чтобы ROC AUC на отложенном тесте получился выше 77.5%. Необходимо интерпретировать результаты модели: важность входящих в нее переменных, демонстрация на нескольких примерах, почему получился соответствующий прогноз. Самое главное, понять какой пол к какому из таргетов (0/1) принадлежит.

Полный набор данных составлен из нескольких файлов: 
## Описание файлов
- transactions.csv - исторические транзакции банковских клиентов
- gender.csv - информация по полу для части клиентов (null - для тестовых)
- tr_mcc_codes.csv - mcc-коды транзакций
- tr_types.csv - типы транзакций

## Описание полей
### transactions.csv
- customer_id - идентификатор клиента
- tr_datetime - день и время совершения транзакции (дни нумеруются с начала данных)
- mcc_code - mcc-код транзакции
- tr_type - тип транзакции
- amount - сумма транзакции в условных единицах; со знаком "+" — начисление средств клиенту, "-" — списание средств
- term_id - идентификатор терминала

### gender.csv
- customer_id - идентификатор клиента
- gender - пол клиента (пустые значения - тестовые клиенты)

### tr_mcc_codes.csv
- mcc_code - mcc-код транзакции
- mcc_description - описание mcc-кода транзакции



Work continues...
