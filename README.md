*Задача решена в рамках ВК-практики*


[A] Предскажи пол(https://cups.online/ru/tasks/1923)
__Задача - разработать модель машинного обучения, которая будет предсказывать пол пользователя соцсетей. Это необходимо, чтобы реклама была эффективной: демонстрировалась пользователям соответствующего гендера.__


***COДЕРЖАНИЕ:***
geo_info, referer_vectors, test, test_users, train_labels, train_part1, train_part2 - исходные данные, я их подгружала сразу в Google Colab

test_result - предсказания модели на test.csv

*Описание датасета  Таблицы*

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







