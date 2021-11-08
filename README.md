# Automated-Testing-Foundations-with-Java

01.MavenBuildTool

1) Установите мавен убедитесь, что он работает.
2) Загрузите тестовый проект отсюда https://github.com/vitalliuss/helloci/tree/master/Java  и соберите его мавеном с помощь цели test
3) Найдите библиотеки junit в папке c:\Users\User_Name\.m2\repository\ и посмотрите на дату создания файлов
4) Измените версию junit в файле pom.xml c 4.12 на 4.11 и соберите проект снова. Проверьте, что новая версия библиотеки добавилась в .m2/repository

02.Jenkins

I Can Win 
1. Установите Jenkins
2. Создайте задачу, которая будет делать следующее:
Клонировать проект https://github.com/vitalliuss/helloci
Запускать тесты из проекта в директори Java с помощью цели mvn test
3. Настройте билд триггеры таким образом, чтобы задача выполнялась раз в 5 минут

Bring It On 
1. Установите Jenkins
2. Создайте задачу которая будет делать следующее:
Клонировать проект https://github.com/vitalliuss/helloci
Запускать тесты из проекта в директори Java с помощью цели mvn test
3. Настройте билд триггеры:
Запуск тестов не позднее чем через 5 минут после коммита в git
Каждый будний день в полночь
4. Опубликуйте файл “Java\target\surefire-reports\com.github.vitalliuss.helloci.AppTest.txt” как артефакт

Hurt Me Plenty 
Данное задание выполняется на основе Bring It On задачи.
1. Сменить порт сервера на 8081
2. Создать ноду и настроить сервер так, чтобы джоба выполнялась только на slave ноде
3. Настроить Job Config History и thinBackup

Hardcore 
Данное задание выполняется на основе Hurt Me Plenty
1. Создать пользователя user и дать ему права на просмотр джоб Jenkins, но без возможности записи или смены настроек
2. Создать параметризованную джобу HelloUser, которая будет спрашивать в качестве параметра имя пользователя (username) и писать в консоль "Hello, username!".
3. С помощью цели  mvn cobertura:cobertura измерьте покрытие кода юнит-тестами (code coverage) и опубликуйте на странице джобы в виде графика
