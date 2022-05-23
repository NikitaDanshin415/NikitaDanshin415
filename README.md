<h1 align="center">Привет! Меня зовут Никита
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">Я работаю инженером по автоматизации тестирования с 2018 года</h3>

### Cтек технологий

<a href="#"><img title="Java" src="logo/java.svg" width="30px"/></a>
<a href="#"><img title="Gradle" src="logo/Gradle.svg" width="50px"/></a>
<a href="#"><img title="JUnit5" src="logo/JUnit5.svg" width="50px"/></a>
<a href="#"><img title="Selenide" src="logo/Selenide.svg" width="50px"/></a>
<a href="#"><img title="Rest-Assured" src="logo/Rest-Assured.svg" width="50px"/></a>
<a href="#"><img title="Allure_Report" src="logo/Allure_Report.svg" width="50px"/></a>
<a href="#"><img title="Docker" src="logo/Docker.svg" width="50px"/></a>
<a href="#"><img title="Jenkins" src="logo/Jenkins.svg" width="50px"/></a>
<a href="#"><img title="Selenoid" src="logo/Selenoid.svg" width="50px"/></a>

### Образование

 <table width="100%" cellspacing="0" cellpadding="5">
    <tr >
        <td align="center"><a href="http://qa.guru/" target="_blank" rel="noopener noreferrer"><img style="width:150px" src="img/qaGuru.svg"></a></td>
        <td>Школа инженеров по автоматизации тестирования QA.GURU.</td>
        <td>2022</td>
    </tr>
    <tr>
        <td align="center">
            <a href="https://perm.hse.ru/" target="_blank" rel="noopener noreferrer"><img style="width:90px" src="/img/01_Abbreviation_ENG_PANTONE.svg"></a>
        </td>
        <td>
            НИУ "Высшая школа экономики".
         <br><b>Программная инженерия.</b>
        </td>
        <td>2018 - 2022</td>
    </tr>
    <tr>
        <td align="center">
            <a href="https://itcollege59.ru/" target="_blank" rel="noopener noreferrer"><img style="width:150px" src="/img/itCollege59.svg"></a>
        </td>
        <td>
            Академическая школа информационных технологий.
         <br><b>Программирование в компьютерных системах.</b>
        </td>
        <td>2015 - 2018</td>
    </tr>
</table>

<a href="#"><img src="https://github-readme-stats.vercel.app/api?username=NikitaDanshin415"/></a>
<a href="#"><img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=NikitaDanshin415&theme=nord_bright"/></a>
<img align="right" src="https://komarev.com/ghpvc/?username=NikitaDanshin415&color=003140">

<h2>Примеры работ:</h2>
<h3>Тесты для Pikabu</h3>
https://github.com/NikitaDanshin415/PikabuTests
<h2><a name='projectStack'>:cookie:Стек проекта:</a></h2>
<p align="center">
    <a href="#"><img title="Java" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/java.svg" width="30px"/></a>
    <a href="#"><img title="Gradle" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/Gradle.svg" width="50px"/></a>
    <a href="#"><img title="JUnit5" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/JUnit5.svg" width="50px"/></a>
    <a href="#"><img title="Selenide" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/Selenide.svg" width="50px"/></a>
    <a href="#"><img title="Allure_Report" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/Allure_Report.svg" width="50px"/></a>
    <a href="#"><img title="Jenkins" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/Jenkins.svg" width="50px"/></a>
    <a href="#"><img title="Selenoid" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/Selenoid.svg" width="50px"/></a>
    <a href="#"><img title="Allure Test Ops" src="https://github.com/NikitaDanshin415/NikitaDanshin415/blob/main/logo/AllureTestOps.svg" width="50px"/></a>
</p>

<ul>
	<li>Java - используется как основной язык для написания тестов</li>
	<li>Gradle - используется для сборки проекта</li>
	<li>Junit5 - тестовый фремворк</li>
	<li>Selenide - библиотека для работы с UI элементами страницы</li>
	<li>Allure - для формирования отчетов</li>
	<li>Jenkins - используется для запуска тестов</li>
	<li>Selenoid - используется для создания контейнеров для прохождения тестов</li>
	<li>AllureTestOps - система управления тестовыми сценариями</li>
</ul>



<h2>:cookie:<a name='projectArchitecture'>Архитектура проекта</a></h2>
Архитектура проекта состоит из 5 основных модулей
<ol>
    <li>
        <b>OwnerConfig</b> - конфигурационные файлы проекта, в которых может содержаться информация о среде выполнения теста и данные необходимые для работы теста.
        Данные для конфига берутся из .properties файла в ресурсах проекта, а так же из параметров запущенного теста.
    </li>
    <li>
        <b>BaseTest</b> - базовый класс с конфигурацией от которого наследуются все классы с тестами. Содержит методы BeforeEach и AfterEach.
    </li>
    <li>
        <b>Test</b> - класс описывающий логику работы теста основываясь на бизнесс требованиях.
    </li>
    <li>
        <b>PageObjects</b> - класс для описания страницы приложения. Поля класса объявляются как приватные константы и описывают селекторы для необходимых элементов.
        Взаимодействие с классом происходит за счет публичных методов класса, использующих ранее описанные селекторы.
    </li>
    <li>
        <b>PageElements</b> - класс для описания логики работы с часто используемыми элементами страницы. (ComboBox, Calendar...)
    </li>
</ol>

```mermaid
flowchart LR
    classDef class1 fill:#ffe0a1
    classDef class2 fill:#f3f76a
    classDef class3 fill:#feffd4
    
	A[Test]:::class1 -.Использует.-o B[PageObject]:::class2
	B -.Использует.-o C[PageElements]:::class3
	A -.Берет данные из.-x D[OwnerConfig]
	A --Наследуется от--> E[BaseTest]:::class1
	E -.Берет данные из.-x D
```
