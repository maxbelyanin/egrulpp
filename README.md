# egrulpp - EGRUL Pdf Parser

Parser for pdf files retreives from [egrul.nalog.ru](https://egrul.nalog.ru).

The parsing result is the object with entity data (Legal entity or Sole entity).

**LE**:
```json
{
    "type": "LE",
    "name": {
        "full": "ОБЩЕСТВО С ОГРАНИЧЕННОЙ ОТВЕТСТВЕННОСТЬЮ \"РОГА И КОПЫТА\"",
        "short": "ООО \"БИЗНЕС-ДОК\""
    },
    "addr": {
        "postcode": "300000",
        "region": "ОБЛАСТЬ ТУЛЬСКАЯ",
        "city": "ГОРОД ТУЛА",
        "street": "УЛИЦА ИВАНОВА",
        "build": "0"
    },
    "reg": {
        "ogrn": "1077123456789",
        "regdate": "01.01.2001"
    },
    "fns": {
        "inn": "7101234567",
        "kpp": "710123456",
        "ifns": "МЕЖРАЙОННАЯ ИНСПЕКЦИЯ ФЕДЕРАЛЬНОЙ НАЛОГОВОЙ СЛУЖБЫ № 11 ПО ТУЛЬСКОЙ ОБЛАСТИ"
    },
    "pfr": {
        "regnum": "081000123456",
        "dpfr": "ГОСУДАРСТВЕННОЕ УЧРЕЖДЕНИЕ - УПРАВЛЕНИЕ ПЕНСИОННОГО ФОНДА РОССИЙСКОЙ ФЕДЕРАЦИИ ПО ПРОЛЕТАРСКОМУ РАЙОНУ Г.ТУЛА"
    },
    "fss": {
        "regnum": "710000123456789",
        "dfss": "ГОСУДАРСТВЕННОЕ УЧРЕЖДЕНИЕ - ТУЛЬСКОЕ РЕГИОНАЛЬНОЕ ОТДЕЛЕНИЕ ФОНДА СОЦИАЛЬНОГО СТРАХОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ"
    },
    "head": {
        "surname": "ИВАНОВ",
        "name": "ИВАН",
        "patronymic": "ИВАНОВИЧ",
        "inn": "710012345678",
        "position": "ДИРЕКТОР",
        "phone": "(0000)123456"
    }
}
```

**SE (IP)**:
```json
{
    "type": "SE",
    "kind": "IP",
    "name": {
        "full": "ИНДИВИДУАЛЬНЫЙ ПРЕДПРИНИМАТЕЛЬ ИВАНОВ ИВАН ИВАНОВИЧ",
        "short": "ИП ИВАНОВ И.И."
    },
    "citizenship": {
        "citizenship": "гражданин Российской Федерации"
    },
    "reg": {
        "ogrn": "304710123456789"
    },
    "fns": {
        "inn": "710012345678",
        "ifns": "МЕЖРАЙОННАЯ ИНСПЕКЦИЯ ФЕДЕРАЛЬНОЙ НАЛОГОВОЙ СЛУЖБЫ № 11 ПО ТУЛЬСКОЙ ОБЛАСТИ"
    },
    "pfr": {
        "regnum": "081000123456",
        "dpfr": "ГОСУДАРСТВЕННОЕ УЧРЕЖДЕНИЕ - УПРАВЛЕНИЕ ПЕНСИОННОГО ФОНДА РОССИЙСКОЙ ФЕДЕРАЦИИ ПО ЗАРЕЧЕНСКОМУ РАЙОНУ Г.ТУЛА"
    },
    "head": {
        "surname": "ИВАНОВ",
        "name": "ИВАН",
        "patronymic": "ИВАНОВИЧ",
        "sex": "мужской"
     }
 }
```

**SE (KFH)**:
```json
{
    "type": "SE",
    "kind": "KFH",
    "name": {
        "full": "ГЛАВА КРЕСТЬЯНСКОГО (ФЕРМЕРСКОГО) ХОЗЯЙСТВА ИВАНОВ ИВАН ИВАНОВИЧ",
        "short": "ГЛАВА КФХ ИВАНОВ И.И."
    },
    "citizenship": {
        "citizenship": "гражданин Российской Федерации"
    },
    "reg": {
        "ogrn": "304710123456789"
    },
    "fns": {
        "inn": "710012345678",
        "ifns": "МЕЖРАЙОННАЯ ИНСПЕКЦИЯ ФЕДЕРАЛЬНОЙ НАЛОГОВОЙ СЛУЖБЫ № 11 ПО ТУЛЬСКОЙ ОБЛАСТИ"
    },
    "pfr": {
        "regnum": "081000123456",
        "dpfr": "ГОСУДАРСТВЕННОЕ УЧРЕЖДЕНИЕ - УПРАВЛЕНИЕ ПЕНСИОННОГО ФОНДА РОССИЙСКОЙ ФЕДЕРАЦИИ ПО ЗАРЕЧЕНСКОМУ РАЙОНУ Г.ТУЛА"
    },
    "head": {
        "surname": "ИВАНОВ",
        "name": "ИВАН",
        "patronymic": "ИВАНОВИЧ",
        "sex": "мужской"
     }
 }
```
