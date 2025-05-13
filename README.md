# Величко Дмитро ІПЗ 3.02
# Практично-лабораторне заняття №6
## Розробка UI для реалізації CRUD-операцій

Склонував проект
![git_clone](https://github.com/user-attachments/assets/9b3201ee-32a4-4ea8-b83b-3fcc84322f77)


Так встановимо деякі залежності у наш проект. 

По-перше напишемо команду ```npm install``` для встановлення деяких залежностей

![npm_install](https://github.com/user-attachments/assets/58c31578-f0cc-4211-89fa-9c5a58695f6f)


як бачимо тут помилки, вони полягають у тому, що проблема з версіями залежностей.

Підемо жорстким шляхом проігноруючи версії акетів. Виконаємо команду: ```npm install --legacy-peer-deps```

![npm_install_--legacy-peer-deps](https://github.com/user-attachments/assets/b4c57d57-1f82-4b3f-b5a4-c91289946ed2)


Тепер запустимо наш проект виконавши команду ```npm run dev```

![npm_run_dev](https://github.com/user-attachments/assets/436d591a-d90d-45b1-bf7b-32d891b636a2)


Тепер ми можеио перейти за адресою ```http://localhost:5173/```

![hello_world](https://github.com/user-attachments/assets/bd90d0f0-24a2-4670-887e-d291ea059cb2)


## 1. Сторінка колекції екземплярів сутності (/posts). 2. Сторінка окремого екземпляра сутності (/posts/:id або /posts/new)

Так спочатку створемо наші сторінки. Перед цим зайдемо у каталог /components/ui створемо
2 файла EntityCard і Modal і створемо у цих каталогах 2 файла у форматі .tsx і.ts

![component_ui](https://github.com/user-attachments/assets/2e58cfab-3d9c-43ab-8e8a-118497bde7aa)

Тепер зміст файлів

# ```EntityCard.tsx```
![entitycard_1](https://github.com/user-attachments/assets/42915147-dffb-417d-ba6e-b88c5a0837b4)
![entitycard_2](https://github.com/user-attachments/assets/93de5d38-7a45-4740-9437-47665db12e7d)


# ```index.ts```
![entitycard_index](https://github.com/user-attachments/assets/cf19d3a0-d835-4fe5-815c-731c7a138180)


# ```Modal.tsx```
![modal](https://github.com/user-attachments/assets/a57bc225-a1cd-4df1-b912-56c06b9ead09)


# ```index.ts```
![modal_index](https://github.com/user-attachments/assets/9ac4bc96-8df2-4adc-97f3-e8b70ebe3d6d)


Так тепер перейдемо у каталог pages створимо три файла: ```Entities.tsx```, ```EntityCreate.tsx```, ```EntityDetails.tsx```

![pages](https://github.com/user-attachments/assets/fe1e11a5-7213-4143-8e27-a25aab23b81f)


# ```Entities.tsx```
![entities_1](https://github.com/user-attachments/assets/bdaa1c02-4a12-4fef-949a-041220408e13)

![entities_2](https://github.com/user-attachments/assets/5dc139d3-4443-44db-8e0b-b6fd0628c017)

![entities_3](https://github.com/user-attachments/assets/17660010-4bf9-4e31-9919-3b70d7f074d1)


# ```EntityCreate.tsx```
![entities_create_1](https://github.com/user-attachments/assets/76f625fc-c981-481c-b082-845bdcf3ebd7)
![entities_create_2](https://github.com/user-attachments/assets/e9d000f5-dccd-4b28-b619-f9be62b61701)
![entities_create_3](https://github.com/user-attachments/assets/9fa1c1ca-b04c-4c35-9799-111504b2e7e1)


# ```EntityDetails.tsx```
![entity_details](https://github.com/user-attachments/assets/e8dcd7dd-f2f9-4a62-97ef-8208177839aa)

Тепер пейдемо у папку routes створимо файл entities з 3 файлами: ```$id.ts```, ```index.ts```, ```new.ts```
![routes](https://github.com/user-attachments/assets/3de5f133-434a-4377-b171-2bf2a1f1d178)

# ```$id.ts```
![id](https://github.com/user-attachments/assets/0e432930-c9be-4267-8b85-3cc649eb1ecd)


# ```index.ts```
![index](https://github.com/user-attachments/assets/718f96c0-0e5e-4a9c-b0fc-fe75a8a4eacf)

# ```new.ts```
![new](https://github.com/user-attachments/assets/ea3715ab-9a83-4ed9-a82c-6896dad35f68)


У файл ```routeTree.gen.ts``` додамо шляхи до роутера:
![routeTree_1](https://github.com/user-attachments/assets/fdaca435-5508-46c8-bc5b-fbb60e8b9c99)
![routeTree_2](https://github.com/user-attachments/assets/1fcffdea-80d2-4642-bc68-01f0ab47e500)
![routeTree_3](https://github.com/user-attachments/assets/c90fa456-7fa3-4258-b20c-9795bee75cf5)
![routeTree_4](https://github.com/user-attachments/assets/08a848b6-56cc-4cd0-b2ff-396459025591)
![routeTree_5](https://github.com/user-attachments/assets/3d5746db-46c7-4a5b-8be3-0a0628c09b78)



У  каталозі ```src``` створемо каталог ```entities``` файл ```index.ts``` де ми напишемо мок-функції

![mock_function](https://github.com/user-attachments/assets/5e92106d-6c66-4fed-82b6-fbbfa1b6aefd)

У каталозі ```src``` створемо каталог ```types``` і створемо файл ```Entity.ts```

![types](https://github.com/user-attachments/assets/2856fe07-759f-4e53-8965-b034d4698cbb)

Тепер запустимо наш проект, для цього в терміналі напишемо команду: ```pnpm run dev```

![result](https://github.com/user-attachments/assets/978363c1-46df-475e-a4f5-ea6c37739c76)

## Створення нової сутності
У кінці сторінки натиснемо кнопку `Додати` і відкриється таке вікно:

![create](https://github.com/user-attachments/assets/f630ea69-2df2-4d78-b87c-2f351b327b5d)

## Поява нової сутності 
![new_entities](https://github.com/user-attachments/assets/4509cc59-d793-4460-909d-e69432174f9b)

## Детальна інформація про сутність

Натиснемо кнопку `Детально` і отримаємо детальну інформацію про сутність

![about](https://github.com/user-attachments/assets/7ecc13f1-8f16-42b7-881b-427ac7131ea6)

## Зміна сутності

Натиснемо кнопку `Редагувати` і нам випаде `prompt` вікно:

### Оновлення назви:

![update_name](https://github.com/user-attachments/assets/1312e83a-79d4-4b7c-8818-418787b1ace7)

### Оновлення опису

![update_desc](https://github.com/user-attachments/assets/c4f06ade-364d-445a-b518-56329b38a3b1)

### Оновлений список

![update_entities](https://github.com/user-attachments/assets/d47cf52b-0ac8-4b8d-8933-955c2d6ba9a9)

## Видалення сутності

Для цього натиснемо кнопку `Видалити`

### Підтвердження видалення

![confirm](https://github.com/user-attachments/assets/c73dc165-694d-428e-8a74-7d854505471e)

### Видалення сутності

![delete](https://github.com/user-attachments/assets/129a44aa-ad1e-4b50-84d6-d1abf40a0897)


## Оновлений список після видалення
![update_list](https://github.com/user-attachments/assets/f9039d58-999c-47e4-ae8a-8c4d8cdf0c13)


## Загальний висновок

У ході практично-лабораторного заняття №6 було повністю реалізовано UI для виконання CRUD-операцій (створення, читання, оновлення та видалення) над сутностями. Було пройдено повний цикл розробки:
- Склоновано та налаштовано проект із відповідними залежностями;
- Успішно вирішено проблеми сумісності за допомогою ```--legacy-peer-deps```;
- Реалізовано компонентну структуру інтерфейсу (компоненти ```EntityCard```, ```Modal```);
- Створено сторінки для перегляду списку сутностей, створення нових, перегляду деталей та редагування;
- Налаштовано маршрутизацію для навігації між сторінками;
- Створено типи та мок-дані для роботи з даними;
- Перевірено функціональність додавання, редагування та видалення сутностей з оновленням списку у режимі реального часу.

Проєкт працює стабільно, відповідає принципам SPA (Single Page Application), а інтерфейс дозволяє зручно керувати сутностями. Ця робота є хорошою практикою у створенні сучасних UI-додатків з React та TypeScript.
