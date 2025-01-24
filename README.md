# wb-tech-school-ab-game

Определим рассматриваемые гипотезы: 

$H_0$: изменения нет

$H_a$: изменение есть

## Эксперименты
Сначала пробегусь по экспериментам, которые я делал, и выводам по каждому из них. Из скринов я привожу скрин лишь лучшего результата, дабы не засорять отчет (я указывал ФИО после эксперимента, так что все цифры, которые я привожу подлинны, и их можно проверить).


### Начальный эксперимент
Первый мой результат был: доход ≈718.000 и конверсия 11.84% (P.S. далеко не рекорд).
В начале эксперимента я заметил, что когда проводишь тест прибыль не меняется, хотя логично, что изменение для части пользователей видно, и прибыль должна меняться (а не быть каждый день по 5000) - по сути тесты можно хоть вплоть до 90-го дня держать, и ничего не поменяется, если их не выкатывать на всех пользователей.

Также я понял следующее: у нас есть 90 дней на максимизацию выручки ⇒ в конце (с ≈80-го дня) нет смысла брать большие релизы, т.к. не хватит времени разработчикам на разработку таких задач и нам на проведение эксперимента.

### Эксперименты со сложностью задач
Интересно узнать, выгоднее отдавать приоритет большим задачам или маленьким. 
Понятно, что первые дольше делаются, но имеют “больший шанс на удачный эксперимент”. Тут конечно есть проблема того, что “большие релизы” / “мелкие доработки” заканчиваются и приходится брать другие задачи, но раз у нас есть возможность попробовать посмотреть на результаты такого эксперимента, надо бы ей воспользоваться. 

Сначала я отдавал приоритет взятию бОльших задач (кроме последних дней разумеется), но так я получил меньшую прибыль (≈647.000) по сравнению с экспериментом начальным экспериментом (≈718.000). Вероятно, сказалось большое количество времени на разработку +, конечно, рандом ⇒ меньшее количество экспериментов ⇒ меньше возможностей для увеличения дохода. 

Теперь я решил отдавать приоритет взятию более маленьких задач (однако все равно были и большие по причине того, что из-за рандома маленькие задачи заканчиваются, и приходится брать большие), я получил наибольший до текущего момента доход в ≈754.000.
Меня удивил данный результат, и я решил еще раз проверить, и в итоге получилось следующее:

<div align="center">
  <img src="https://github.com/user-attachments/assets/3de35597-8fe3-488d-bd0b-bf2ca216d25b" alt="table" style="width:70%;">
</div>

Так я получил наибольший доход за все эксперименты ≈`929.000` и наибольшую конверсию `18.21%`.

<div align="center">
  <img src="https://github.com/user-attachments/assets/8ab21529-3df0-4a74-b0a4-d6a17a30cb91" alt="big big">
</div>

Что же нам говорят данные эксперименты? Скорее всего, из-за рандома мы можем как при взятии больших задач, так и маленьких получать бОльший доход и бОльшую конверсию. Но стоит отметить, что в первом случае у нас на последние дни копятся именно маленькие задачи, что очень удобно (ведь большие релизы просто не успеют разработать, а мы не успеем доделать такие эксперименты).

### Эксперимент с одинаковыми командами
Также я хотел проверить, стоит ли проводить эксперимент так, чтобы задачи отделов не пересекались ⇒ соответственно, группы пользователей тоже.

В этом эксперименте старался брать задачи так, чтобы они пересекались, например так:
<div align="center">
  <img src="https://github.com/user-attachments/assets/9c38b073-dc01-4d82-ba4c-2738cd22d065" alt="photo" style="width:55%;>
</div>div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/ca6e330c-513a-4728-b7d4-5fe3c0263ddc" alt="table2" style="width:50%;">
</div>
    
Ожидаем, что если нужно брать *непересекающиеся* задачи, то мы серьезно порежем доход начального эксперимента ≈718.000 и его конверсию 11.84%. 

Проведя 2 эксперимента с пересекающимися задачами, получили вышеуказанные результаты. Да, доход упал, но не на сотни тысяч. Проведя немало экспериментов, сложилось четкое впечатление, что рандом очень влияет (логично, что если в начале 
эксперимента мы получаем выгодный для нас тест, то все дни после его релиза мы будем получать бОльший доход), и резонно предположить, что здесь также (мы уже видели немалые скачки дохода в прошлом разделе, когда смотрели на сложность задач). Поэтому сложно утверждать, что обязательно нужно брать непересекающиеся задачи отделов в этой игре (разумеется, в реальной работе аналитика важно, чтобы эксперименты не влияли друг на друга).

### Сравнение длительности экспериментов

Я провел эксперименты с разными *фиксированными* длительностями тестов: 3, 7, 10, 14 дней. 

Результаты:
<div align="center">
  <img src="https://github.com/user-attachments/assets/356363a9-82e0-4e3a-b996-e80634435d29" alt="V">
</div>

Очевидно, что если нам интересно максимизировать прибыль, то фиксация момента, когды мы принимаем решение, нам в данной игре (подчеркиваю, что не в реальной жизни) не помогает.


## Выводы
- Всегда даем разработчикам задачи (для этого, удобно держать в разделе “взято в работу” 3+ задачи).
- С ≈80-го дня не берем большие релизы (для этого можно стараться брать большие заказы, тогда на конец останутся маленькие - как раз так я достиг максимальной прибыли)
- Я говорил ранее, что при проведении эксперимента прибыль не меняется в зависимости от изменений, сделанных для тестовой группы эксперимента ⇒ ухудшение конверсии в экспериментах нас не пугает в плане того, что нужно резко все прерывать; и длительные тесты не несут для нас финансовых потерь в этой игре. 
- По истечении длительности эксперимента принимаем решение следующим образом:
<div align="center">
<img src="https://github.com/user-attachments/assets/77797ade-821f-4ce4-9cf1-de997ca44b6b" alt="решение (1)" style="width:100%;">
</div>

- Хороший вопрос, что есть длительность. В реальной жизни, если условно идет речь рекомендациях, мы хотя бы понимаем, что именно за рекомендации ⇒ есть хоть какие-то основания для выбора определенной длительности теста ⇒ именно по прошествии заданного количества дней принимаем решение (если конечно мы прям ужасно все метрики не занизили и не приняли решение прервать эксперимент); а здесь все, что знаем - это название команды, которая делает изменение. В нашей игре, конечно, можно зафиксировать срок длительности теста, но я показал выше, что в таких случаях денег мы больше не зарабатываем, а у нас задача максимизировать прибыль. В общем, в условиях ограниченного функционала для получения максимальной прибыли, как и было сказано в задании, лучше ждать несколько дней и убеждаться в том, что эксперимент увеличивает доход.
