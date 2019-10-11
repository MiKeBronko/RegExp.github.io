# RegExp.github.io
## Sprint 10 - pattern Regular expression
### student - Mikhail Fatkin
#### HTML
(https://mikebronko.github.io/RegExp.github.io/ "this project you can see :--)")

# aLSO
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Regular Expressions</title>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <header class="header">
        <img class="header__logo" src="https://pictures.s3.yandex.net/frontend-developer/dom_bom/logo.svg" alt="logo">
        <p class="header__logo-sub">Регулярные выражения</p>
    </header>
    <main class="container">
        <div class="cover">
            <div class="cover__image"></div>
            <h1 class="cover__heading">RegExp</h1>
        </div>
        <div class="block">
            <form novalidate class="form" name="register" action="http://httpbin.org/post" method="POST">
                <h3>Форма регистрации</h3>
                <fieldset class="form__fieldset">
                    <div class="form__field">
                        <input class="form__input" type="text" name="name" pattern="^[А-ЯЁ][А-ЯЁа-яё-]+$" placeholder="Имя" required minlength="2" maxlength="20"/>
                    </div>
                    <div class="form__field">
                        <input class="form__input" type="email" name="name" pattern="^[\w\.-]+@[a-z-]+\.[\w]{2,6}$" placeholder="E-Mail" />
                        <span class="form__error">e-mail в формате: sega@yandex.ru</span>
                    </div>
                    <div class="form__field">
                        <input class="form__input" type="tel" name="name" placeholder="Телефон" pattern="^(\s*)?(\+)?([- _():=+]?\d[- _():=+]?){10,14}(\s*)?$" minlength="" maxlength="" />
                        <span class="form__error">телефон в формате: +7 (123) 456-78-90</span>
                    </div>
                    <div class="form__field">
                        <input class="form__input" type="url" name="name" pattern="^((http|https):\/\/)?(www\.)?([A-Za-zА-Яа-я0-9]{1}[A-Za-zА-Яа-я0-9\-]*\.?)*\.{1}[A-Za-zА-Яа-я0-9-]{2,8}(\/([\w#!:.?+=&%@!\-\/])*)?" placeholder="Ваш сайт" />
                        <span class="form__error">URL в формате: http://mysite.ru</span>
                    </div>
                    <button class="form__button" type="submit">Отправить</button>
                </fieldset>
            </form>
        </div>
    </main>     
</body>
</html> 