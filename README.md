# Java Backend дастурчиси билимини бахолаш учун топшириқ

Сизга тақдим этилаётган ушбу лойиҳа **duol.uz** жамоси тамонидан ишлаб чиқилган. 
Мазкур лойиҳадан кўзланган асосий мақсад бизнинг компаниямизга `Java Backend` дастурчи сифатида ишга киришни истаги бўлган 
номзодларнинг билим даражасини, технологиялардан тўғри фойдалана олишини, ҳамда код ёзиш услуби ҳақидаги маълумотларни аниқлаш
ҳисобланади.

![](https://i.ibb.co/FxBtfQ4/duol-logo.png)

### Лойиҳани ҳақида қичқача маълумот
Сиздан Java Spring дастурчичи сифатида талаб қилинадиган лойиҳа бу Spring Boot ёрдами оддий веб иловани ишлаб чиқиш ҳисобланади.
Мазкур лойиҳа java ва Spring ҳақида мақолалар ва уларга ёзиладиган шрахлардан ташкил топган ва унинг номни BLOG деб номалймиз.
Ушбу лойиҳада ассоан ўрганувчилар учун долзарб ва қизиқарли бўлган маълумотлар тўлиқ ёртииб борилади. 

Топшириқ ҳақидаги тўлиқ маълумотларни сиз [PROJECT_REQUIREMENTS](/PROJECT_REQUIREMENTS.md) файлидан олшингиз мумкин.



### Лойиҳани амалга ошириш бўйича қичқача маълумот

Мазкур лойиҳа сизниг Java дастурлаш тили ҳақида билимларингизни аниқлаш ҳамда замонваий технологиялар ечимларни қай 
даражада қўллай олишингиз ҳақидаги маълумотларни аниқлаш учун мўлжалланган. Сизларга енгиллик яратиш мақсадида енгил 
ва ўртача даражадаги технолигиялардан фойдаланишга қарор қилдик.
Яъни лойиҳани амалга оширишда сиз қуидагилардан фойдаланишингиз мумкин:

* **Java 8+**
* **Spring Boot**
* **Spring Data JPA**
* **Thymeleaf** (MVC андозаси асосида яратилган лойиҳа бўлганлиги сабали HTML ёрдамида маълумотларни акс эттириш учун)
* **PostgreSQL** (Бошқа бир DBMS типидаги маълумотлар базасидан хам фойдаланиш мумкин)
* **Maven** (Лойиҳа таркибидаги боғликларни бошқариш, йиғиш, тетс синовидан ўткази ва ишга тушириш учун)

## Git Commit ҳақида
Ушбу ҳужжат git commit учун ёзиладан хабарлар ва шарҳлар учун қоидалар тўпламидан ташкил топган.
Лойиҳанинг ҳар бир иштирокчиси қуйидаги қоидаларни яхши билиши талаб этилади.

Бизнинг жамода git commit ҳабарларини ёзиш формати бўйича аниқ ишлаб чиқилган қоидаларимиз бор.
Бу қоидалар бизга лойиҳанинг тарихини кузатишни енгиллаштиради ҳамда мазкур ўзгаришлар ҳақида хабарларни ўқишни осонлаштиради.

## Git Commit ҳақидаги хабарларни форматлаш бўйича наъмуна

Ҳар битта Git Commit хабари сарлавҳа, асоси қисм ва пастки қисмдан ташкил топган
The header has a special format that includes a type, a scope and a subject:
Сарлавҳа ҳам ўзнавбатида махсус форматга эга бўлиб, у топшириқ тури ва унинг мавзусини ўз ичига қамраб олади
Хабарлар қуйида келтирилган намуна асосида яратилади:
```gitexclude
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

Бу ерда сарлавҳа(subject)ни тўлдириш мажбурий ва топшириқ тури(scope)ни белгилаш ихтиёрий ҳисобланади.
Шунингдек ҳар қандай хабардаги символлар сони 100 та символдан ошмаслиги лозим.
Бу жиҳат бизларга турли ҳилдаги git воситалари ёрдамида хабарни ўқиш жараёнини енгиллаштиради.

Лойиҳа доирасида юзага келадиган ўзрашилар турини ифодалаш учун одатда қуйидаги типлардан фойдаланилади:
* **feature**: Лойиҳага янги имклниятлар ёки функциялар амалга оширилган тақдирда фойдаланилади
* **fix**: Лойиҳага тегишли турли хил хатоликларни тўғриланган тақдирда фойдаланилади
* **docs**: Лойиҳага тегишли ҳужжатдар ўзгарган тақдирда фойдаланилади
* **style**: дастурдаги кодларнинг мазмунига таъсир қилмайдиган ўзгаришлар (ортиқча пробелларни олиб ташлаш, форматлаш ва бошқалар)
* **refactor**: Мавжуд коднинг ишлашиши тўғриламайдиган ёки янги фунциялар қўшилмаган тарздаги мавжуд кодларнинг ўзгаришини ифодаш учун ишлатилади
* **perf**: Коднинг иш самарадорлигини яхшилашга қаратилган ўзгаришлани ифодалаш
* **test**: Янг тестларни қўйиш ёки мавжудларини тўғрилнганлигини ифодалаш учун ишлатилади
* **build**: Лойиҳани ишчи ҳолатга келтириш ва йиғишга таъсир қилувчи ўзгаришларни ифодалаш учун ишлатилади (мисол учун: gulp, npm)
* **ci**: CI конфигурацияларига алоқадор файл ва скриптларга киритилган ўзгаришларни ифодалаш учун ишлатилади (мисол учун: Travis, Circle, BrowserStack, SauceLabs)
* **chore**: Лойиҳа таркибидаги src ва test файллари ташқари ўзгаришларни ифодалаш учун ишлатилади
* **revert**: Лойиҳага киритлган ўзгаришларни бекор қилиш олдини ҳолатига қайтариш учун ишлатилади

## Дастурни тетслаш бўйича талаблар

Лойиҳадаги кодларни тестлаш мақсадида сиздан албатта `unit test` талаб этилади.
Testcontainers ассоан интеграция билан боғлиқ тетсларни амалша ошириш учун фойладанилади.

### Лойиҳани амалага ошириш бўйича керакли маълумотлар  

Батафсил маълумотлар билан танишиш учун қуйида келтирилган манбалар билан танишиб чиқишнигзни тавсия қиламиз:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/3.1.2/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/3.1.2/maven-plugin/reference/html/#build-image)
* [Spring Boot Testcontainers support](https://docs.spring.io/spring-boot/docs/3.1.2/reference/html/features.html#features.testing.testcontainers)
* [Testcontainers Postgres Module Reference Guide](https://www.testcontainers.org/modules/databases/postgres/)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/3.1.2/reference/htmlsingle/#using.devtools)
* [Spring Web](https://docs.spring.io/spring-boot/docs/3.1.2/reference/htmlsingle/#web)
* [Validation](https://docs.spring.io/spring-boot/docs/3.1.2/reference/htmlsingle/#io.validation)
* [Testcontainers](https://www.testcontainers.org/)
* [Spring Data JPA](https://docs.spring.io/spring-boot/docs/3.1.2/reference/htmlsingle/#data.sql.jpa-and-spring-data)
* [Flyway Migration](https://docs.spring.io/spring-boot/docs/3.1.2/reference/htmlsingle/#howto.data-initialization.migration-tool.flyway)

### Лойиҳани амалага ошириш бўйича қўлланма

Кйидаги қўлланмалар асосида баъзи бир нозик масалаларга жавоб тошингиз ва ундан қандай фойдаланиш борасидаги маълумотларга эга бўлишингиз мумкин:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [Validation](https://spring.io/guides/gs/validating-form-input/)
* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)

###  Барча номзодларга омад тилаймиз!