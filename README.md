# Правила запуска
Для студентов отдельные ветки. 
Принцип следующие: есть ветвь students, от нее студент создает ветвь
Сервер в основном не связан с клиентом, его можно не запускать, ничего не изменится
## Запуск клиент
1. Для начала создаете аккаунты в Clerk, Convex, Liveblocks с проектами Tula
2. Настройки Clerk - обязательно создайте jwt для convex и активируйте организации:![alt text](image.png)![alt text](image-1.png)![alt text](image-2.png)![alt text](image-3.png)![alt text](image-4.png)![alt text](image-5.png)![alt text](image-6.png)
3. Настройка Convex - в переменные окружения, входа обязательно введите ссылку на clerk jwt:![alt text](image-7.png) ![alt text](image-8.png)
4. Из Liveblocks нам нужны ключи api
5. Все ключи Api меняем в файле .env.local, так же поменяйте ссылку в файле auth.config.ts
6. Сначала запускайте convex, затем клиент 
nextJs - npm run dev
convex - npx convex dev

