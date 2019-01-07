---
tags: ["kovri"]
terms: ["Clearnet", "клирнете", "клирнету", "клирнет"]
summary: "Интернет, в котором построены сети анонимного наложения"
---

### Основная информация

Когда вы пользуетесь Интернетом для того, чтобы, например, узнать новости, отправить почту, пообщаться в соцсетях и даже воспользоваться своими Monero, то, наиболее вероятно, вы используете соединение Clearnet. Это означает, что *все* ваши соединения можно отследить и просмотреть посредством:

- вашего [ISP](https://en.wikipedia.org/wiki/ISP)
- веб-сайта / службы / человека, с которым вы связываетесь
- через организацию, связанную с [Five Eyes](https://en.wikipedia.org/wiki/5_Eyes)

И даже если вы используете [HTTPS](https://en.wikipedia.org/wiki/HTTPS) или подобный протокол (*шифрующий* передаваемые вами данные), ваш маршрут остаётся открытым и не анонимным, то есть *прозрачным* (clear).

### Углублённая информация

Так как традиционный [VPN](https://en.wikipedia.org/wiki/VPN) не может защитить вас от клирнет (так как вы до сих пор находитесь в среде *клирнет* (даже несмотря на то, что вы защищены через прокси сильнее, чем через VPN)), следует использовать *анонимную оверлейную сеть*, которая позволит избежать прямого взаимодействия с Clearnet:

- @Kovri
- @Java-I2P
- [Tor](https://torproject.org/)

Эти технологии защитят вас от клирнета путём построения анонимной сети **поверх** самого клирнета, в результате чего передаваемые вами данные будут как зашифрованными, так **и** анонимными.

Здесь вы можете увидеть [интерактивную диаграмму](https://www.eff.org/pages/tor-and-https), предоставленную [EFF](https://www.eff.org/) и описывающую, как работает *клирнет* и Tor. Эта концепция также (некоторым образом) применима к @Kovri и @I2P с точки зрения анонимности за исключением следующего:

- @Kovri не использует выходных узлов при соединении с @eepsite
- Ваш трафик никогда не выходит за пределы сети @I2P;
- Вам не нужен HTTPS, чтобы использовать @Kovri (за исключением Reseed).