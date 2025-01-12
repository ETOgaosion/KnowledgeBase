---
title: Страницы, защищённые браузером
sidebar_position: 4
---

:::info

Эта статья о Браузерном расширении AdGuard, которое защищает только ваш браузер. Чтобы защитить всё устройство, [скачайте приложение AdGuard](https://adguard.com/download.html?auto=true)

:::

## Страницы, защищённые браузером

When using a web extension like AdGuard Browser Extension, there are certain restricted domains that prohibit access or permissions. В результате расширениям для блокировки рекламы не разрешается изменять содержимое этих страниц. Другими словами, они не могут блокировать рекламу и другие раздражающие элементы на этих веб-страницах.

### Ограничения браузера Chromium

Браузеры на базе Chromium, такие как Google Chrome, ведут список доменов, к которым расширениям запрещён доступ. К таким доменам относятся:

- clients.google.com
- clients[0-9]+.google.com
- sb-ssl.google.com
- URL-адреса, начинающиеся с `chrome://`, `chrome-extension://` или `https://chrome.google.com/webstore/`
- PDF-файлы
- Страницы, на которых отключён Javascript
- Страницы предупреждений о безопасности
- Страницы ошибок, такие как 404 и сетевые ошибки
- URL-адреса, начинающиеся с `view-source:` или `data:`

### Ограничения браузера Firefox

Аналогичным образом, у браузера Firefox есть свой набор доменов с ограничениями, на которых расширениям работать не разрешено. К таким доменам относятся:

- accounts-static.cdn.mozilla.net
- accounts.firefox.com
- addons.cdn.mozilla.net
- addons.mozilla.org
- api.accounts.firefox.com
- content.cdn.mozilla.net
- discovery.addons.mozilla.org
- install.mozilla.org
- oauth.accounts.firefox.com
- profile.accounts.firefox.com
- support.mozilla.org
- sync.services.mozilla.com

### Изменение ограничений в Firefox

Изменение расширенных настроек может повлиять на стабильность и безопасность работы Firefox. Рекомендуется только для опытных пользователей. If you are aware of the associated risk and still wish to enable add-ons disallowed on a protected page, follow the steps below:

1. Click the menu button → **Add-ons and themes** → **Extensions**.
2. Нажмите на расширение, которое вы хотите включить на сайтах с ограничениями (в данном случае AdGuard).
3. В разделе **Запускать на сайтах с ограничениями**выберите **Разрешить**.

Кроме того, вы можете:

1. Открыть новую вкладку и ввести в адресной строке **about:config**.
2. Нажать **Установить**. Может появиться предупреждение. Тогда нажмите **Принять риск и продолжить**.
3. Найдите `расширений.webextensions.restrictedDomains`. Если вы не можете найти эту настройку, то можете создать её. Просто выберите тип **Boolean** и нажмите **+** для его добавления.
4. Измените значение этого параметра на `false`.
5. Перезапустите Firefox.

Более подробную информацию по этому вопросу можно найти в статье [на сайте поддержки Mozilla](https://mzl.la/3POXoWi).
