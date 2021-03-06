# Инструкция по hpool для windows
**от @BMW для Chia Russian Community** - <https://discord.gg/89qT4SuAGm>

1. Регистрируемся на hpool. Подтверждаем свою учетную запись по номеру телефона. (на момент написания инструкции смс в РФ не приходят, можно воспользоваться сервисами для покупки временных сим-карт. Не переживайте, вам этот номер понадобится только при выводе средств, его можно будет поменять на любой перед выводом, но в РФ не придет смс :D универсального решения на данный момент нет. Если найдете – пишите, дополню инструкцию)

2. Скачиваем из центра загрузок `CHIA-plotter`
![screen1](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/1.png?raw=true)
![screen2](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/2.png?raw=true)

3. Здесь вам нужно ввести вашу мнемоническую фразу (много разных слов, которые вы получили при создании кошелька)
![screen3](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/3.png?raw=true)

4. Сверяем наш fingerprint с тем, что написан в Chia Blockchain
![screen4](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/4.png?raw=true)

5. Переходим из личного кабинета в раздел Open Pool. Жмем вверху “All” и переходим к конфигурированию пула
![screen5](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/5.png?raw=true)

6. Забираем подпись, полученную на шаге 3. Вставляем подпись в поле “Bind signature data” и нажимаем кнопку “Bind
![screen6](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/6.png?raw=true)
![screen7](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/7.png?raw=true)

7. Скачиваем Chia Miner (версия 1.0.5 как показали отзывы стабильнее. Я использую 1.1.0)
![screen8](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/8.png?raw=true)

8. Распаковываем архив и запускаем hpool-miner-chia-gui.exe
![screen9](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/9.png?raw=true)

9. В случае с версией 1.0.5 авторизуетесь внутри приложения и переходите к шагу 14. В случае с 1.1.0 и выше следуйте далее.

10. Нажмите на кнопку сверху справа
![screen10](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/10.png?raw=true)

11. Перейдите в раздел конфигурации в личном кабинете и скопируйте API Key.
![screen11](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/11.png?raw=true)

12. Вставьте ключ в открывшемся на 10 шаге окне. И проведите настройку майнера, как показано на скриншоте ниже. Не стоит делать слишком частое обновление директории плотов. По моим наблюдениям, это снижает скорость добычи. Выставьте такое время, за которое у вас появляются новые плоты.
![screen12](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/12.png?raw=true)

13. Добавьте ваши директории плотов. Они должны появиться в таблице ниже. Для каждой новой директории нажимайте кнопку снова и снова.
![screen13](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/13.png?raw=true)
Майнинг запущен. Пропустите шаг 14, если использовали версию 1.1.0 и выше. И перейдите к шагу 15.

14. Для версии 1.0.5
![screen14](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/14.png?raw=true)

15. Важно удалить директории ваших плотов из официального приложения во избежание двойного майнинга. При этом, если вы делаете плоты с помощью официального приложения, ставьте галку «exclude final directory». Так, при создании новых плотов, они не будут добавлены в кошелек, и вы избежите проблему двойного майнинга. 
![screen15](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/15.png?raw=true)
Удалите уже имеющиеся ссылки на директории плотов из официального кошелька:
![screen16](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/16.png?raw=true)
---

После прохождения всех шагов инструкции, проверьте все ли работает на пуле:
![screen17](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/17.png?raw=true)

В разделе “Online Plot” через час-два вы должны увидеть полный список ваших плотов:
![screen18](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/18.png?raw=true)

Если вы все сделали правильно, и у вас все плоты рабочие, вы увидите у каждого плота статус
“signed”. Проверьте, чтобы все плоты были подписаны.

Во вкладке “revenue” вы можете следить за прогрессом начисления ваших наград. Учтите, что вы
получаете награды не за все блоки, которые нашел пул, а только за те, в которых вы приняли
участие. Статус “Unsettlement” будет у всех блоков до тех пор, пока они не будут подтверждены
пулом. Подтверждение происходит ежедневно, в 6:30 утра по Москве.
![screen19](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/19.png?raw=true)

Кучи ваших денег в chia вы можете смотреть в нижней части вкладки “Home”
![screen20](https://github.com/chia-net-ru/HowTo/blob/main/hpool/img/20.png?raw=true)

Вывод средств происходит по кнопке «Withdraw» во вкладке Home. Минимальная сумма к выводу
на момент написания инструкции – 0.2 XCH

## Удачного майнинга!
Благодарить можно монетами XCH сюда -
`xch1gl4d9mj5vgvh9tsv6zws6nqtr639kk3l8mvqm8m28x8gvzeurntq3nnjg4`

Присоединяйтесь к Рускоязычному дискорд сообществу <https://discord.gg/89qT4SuAGm>
