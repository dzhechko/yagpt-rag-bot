## YaGPT чат-бот для работы с pdf-файламм

### Краткая информация
Данный YaGPT-бот реализует [Retrieval-Augmented Generation (RAG)](https://github.com/yandex-cloud-examples/yc-yandexgpt-qa-bot-for-docs/blob/main/README.md) подход
и использует следующие компоненты:
- [Yandex GPT](https://cloud.yandex.ru/services/yandexgpt)
- [Yandex GPT for Langchain](https://pypi.org/project/yandex-chain/)
- [YC MDB Opensearch](https://cloud.yandex.ru/docs/managed-opensearch/)
- [Streamlit](https://streamlit.io/)
- [LangChain](https://python.langchain.com/)

### Структура репозитория и порядок работы с ботом
- в файле ``.env`` находятся системные переменные (которые при запуске в облаке можно указать как secrets)
```
YAGPT_FOLDER_ID = 
YAGPT_API_KEY = 
MDB_OS_PWD = 
MDB_OS_HOSTS = fqdn-host1,fqdn-host2,fqdn-host3
```
- файл `requirements.txt` традиционно содержит в себе список необходимых для работы программы модулей, которые устанавливаются командой 
```pip install -r requirements.txt ```
- в папке `images` хранится логотип компании, который можно использовать в графическом интерфейсе streamlit
- `YaGPT-RAG-bot.py` запускаемый файл
- для упрощения запуска в облаке в исходном коде отключена проверка сертификата на MDB Opensearch

### Запуск в Streamlit Community Cloud
Вы можете развернуть это приложение через Streamlit Community Cloud, следуя [следующим инструкциям](https://docs.streamlit.io/streamlit-community-cloud/get-started)

