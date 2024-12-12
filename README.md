# VK_hack

Группа №13 УрФУ
Участники:
Данил Архипов
Владимир Сергеев
Максимова Наталья
Илона Уткевич

Цель проекта:
Разработать модель машинного обучения, 
которая будет предсказывать пол пользователя соцсетей.

Project Organization
------------
    ├── README.md
    ├── data            <- Папка с файлами из датасета
    ├── experiments     <- Папка с экспериментальными ноутбуками
    ├── hackvk_1.ipynb  <- Файл с EDA
    └── hack_vk_2.ipynb <- Файл с обучением модели 



Описание датасета
Таблицы

train_labels.csv:
- «user_id» - id пользователя;
- «target» - пол пользователя (1 / 0).
 
train.csv, test.csv;
- «request_ts» - server timestamp of request;
- «user_id» - id пользователя (см. п.1);
- «referer» - url, где показывается реклама. В данном случае захэшировано 2 части url:
1) domain - домен урла;
2) path - все что после domain. Например, https://a758bf6/1432d3f1, a 758bf6 - domain, 1432d3f1 - path.
- «geo_id» - id geo;
- «user_agent» - строка user_agent.
 
referer_vectors.csv:
- «component0» - … - «component9» - числа, которые несут в себе информацию о url. Их нельзя как-либо интерпретировать;
- «referer» - url, где показывается реклама (см. п.2).
 
geo_info.csv:
- «geo_id» - id geo (см. п.2);
- «country_id» - id страны;
- «region_id» - id региона;
- «timezone» - часовой пояс для geo.










