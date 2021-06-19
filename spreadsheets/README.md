# Автоматизирейм добавление данных в таблицу

## Формы
https://docs.google.com/forms/d/e/token/viewform?usp=sf_link

## Отправляемые данные
https://docs.google.com/forms/d/e/token/formResponse
```
POST
entry.1228341422: 222
fvv: 1
draftResponse: [null,null,"-5420614843103725440"]
pageHistory: 0
fbzx: -5420614843103725440
```

https://docs.google.com/forms/d/e/token/formResponse
```
entry.1228341422: 333
fvv: 1
draftResponse: [null,null,"9205228334290486864"]
pageHistory: 0
fbzx: 9205228334290486864
```

Content-Type: application/x-www-form-urlencoded

    curl -X POST -F 'entry.1228341422=444' -F 'fvv=1' -F 'draftResponse=%5Bnull%2Cnull%2C%221%22%5D%0D%0A' -F 'pageHistory=0' -F 'fbzx=1' https://docs.google.com/forms/d/e/token/formResponse


## Ситикард
Табличка с добавлением данных curl-ом
https://docs.google.com/forms/d/e/token/viewform?usp=sf_link

curl -X POST -F 'entry.1029311933=15224' -F 'entry.349599747=10576' -F 'fvv=1' -F 'draftResponse=%5Bnull%2Cnull%2C%221%22%5D%0D%0A' -F 'pageHistory=0' -F 'fbzx=1' https://docs.google.com/forms/d/e/token/formResponse
