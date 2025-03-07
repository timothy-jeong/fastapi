# Учебник - Руководство пользователя

В этом руководстве шаг за шагом показано, как использовать **FastApi** с большинством его функций.

Каждый раздел постепенно основывается на предыдущих, но он структурирован по отдельным темам, так что вы можете перейти непосредственно к конкретной теме для решения ваших конкретных потребностей в API.

Он также создан для использования в качестве будущего справочника.

Так что вы можете вернуться и посмотреть именно то, что вам нужно.

## Запустите код

Все блоки кода можно копировать и использовать напрямую (на самом деле это проверенные файлы Python).

Чтобы запустить любой из примеров, скопируйте код в файл `main.py` и запустите `uvicorn` с параметрами:

<div class="termy">

```console
$ uvicorn main:app --reload

<span style="color: green;">INFO</span>:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
<span style="color: green;">INFO</span>:     Started reloader process [28720]
<span style="color: green;">INFO</span>:     Started server process [28722]
<span style="color: green;">INFO</span>:     Waiting for application startup.
<span style="color: green;">INFO</span>:     Application startup complete.
```

</div>

**НАСТОЯТЕЛЬНО рекомендуется**, чтобы вы написали или скопировали код, отредактировали его и запустили локально.

Использование кода в вашем редакторе — это то, что действительно показывает вам преимущества FastAPI, видя, как мало кода вам нужно написать, все проверки типов, автодополнение и т.д.

---

## Установка FastAPI

Первый шаг — установить FastAPI.

Для руководства вы, возможно, захотите установить его со всеми дополнительными зависимостями и функциями:

<div class="termy">

```console
$ pip install "fastapi[all]"

---> 100%
```

</div>

...это также включает `uvicorn`, который вы можете использовать в качестве сервера, который запускает ваш код.

/// note | Технические детали

Вы также можете установить его по частям.

Это то, что вы, вероятно, сделаете, когда захотите развернуть свое приложение в рабочей среде:

```
pip install fastapi
```

Также установите `uvicorn` для работы в качестве сервера:

```
pip install "uvicorn[standard]"
```

И то же самое для каждой из необязательных зависимостей, которые вы хотите использовать.

///

## Продвинутое руководство пользователя

Существует также **Продвинутое руководство пользователя**, которое вы сможете прочитать после руководства **Учебник - Руководство пользователя**.

**Продвинутое руководство пользователя** основано на этом, использует те же концепции и учит вас некоторым дополнительным функциям.

Но вы должны сначала прочитать **Учебник - Руководство пользователя** (то, что вы читаете прямо сейчас).

Он разработан таким образом, что вы можете создать полноценное приложение, используя только **Учебник - Руководство пользователя**, а затем расширить его различными способами, в зависимости от ваших потребностей, используя некоторые дополнительные идеи из **Продвинутого руководства пользователя**.
