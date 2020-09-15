# Пример создания похожего на ЛР 4 клиентского приложения

Сразу стоит оговориться, что это вряд ли можно всерьез назвать клиентским приложением, потому что клиентские приложения устроены куда сложнее и умеют работать с сетью (то есть слать данные на сервер). Пока же наша цель совершенно не состоит в том, чтобы научиться этому всему - мы попытаемся использовать JS по его первоначальному назначению: перерисовывать пиксели в браузере.

Это приложение - пример "чат-бота". Это словосочетание неслучайно взято в кавычки - здесь мы не будем реализовывать вообще никакую сложную интеллектуальную логику - мы будем просто случайно выбирать ответ из соответствующей группы.

Следует обратить самое пристальное внимание на то, как устроена перерисовка. Мы держим в памяти браузера структуру данных и меняем DOM в соответствии с ней. При этом структура данных важнее. Таким образом мы избавляемся от нудных, громоздких и непонятных на первый взгляд итераций по DOM-дереву и как бы "выпячиваем" логику, что всегда хорошо для любого приложения, особенно если речь идет про JS.
