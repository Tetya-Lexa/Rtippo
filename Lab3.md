# Лабораторная работа 3
## Игра в шашки

### Диаграммы последовательности

### Прецедент "Создать игру"

![alt text](<./3.1.jpg>)

| Операция       | Вводит своё имя                                                  |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Создать игру"                                         |
| Предусловие    | Игрок подключен к системе                                        |
| Постусловие    | Система получила имя игрока                                      |

---

| Операция       | Нажимает на кнопку "Создать игру"                                |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Создать игру"                                         |
| Предусловие    | Игрок подключен к системе и ввёл своё имя                        |
| Постусловие    | Комната создана, ожидается подключение второго игрока            |

---

| Операция       | Подключает игрока в комнату для игры                             |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Создать игру"                                         |
| Предусловие    | Игрок нажал на кнопку "Создать игру" и ввёл имя                  |
| Постусловие    | Игрок находится в комнате для игры                               |

### Прецедент "Присоединиться к игре"

![alt text](<./3.2.jpg>)

| Операция       | Нажимает кнопку "Присоединиться к игре"                          |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Присоединиться к игре"                                |
| Предусловие    | Игрок подключен к системе                                        |
| Постусловие    | Игрок присоединён к комнате с игроком                            |

### Прецедент "Сделать ход"

![alt text](<./3.3.jpg>)

| Операция       | Игрок передвигает шашку, делая ход                               |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Сделать ход"                                          |
| Предусловие    | Игрок находится в комнате для игры                               |
| Постусловие    | Игрок передвинул шашку                                           |

---

| Операция       | Убирает шашку противника                                         |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Сделать ход"                                          |
| Предусловие    | Игрок передвинул шашку                                           |
| Постусловие    | Игрок сделал ход и забрал шашку противника                       |

---

| Операция       | Передвигает шашку                                                |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Сделать ход"                                          |
| Предусловие    | Игрок находится в комнате для игры                               |
| Постусловие    | Игрок сделал ход                                                 |

### Прецедент "Признать поражение"

![alt text](<./3.4.jpg>)

| Операция       | Нажимает кнопку "Признать поражение"                             |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Признать поражение"                                   |
| Предусловие    | Игрок находится в комнате для игры                               |
| Постусловие    | Игра закончена                                                   |

---

| Операция       | Сообщение о принятии поражения                                   |
|----------------|------------------------------------------------------------------|
| Ссылки         | Прецедент "Признать поражение"                                   |
| Предусловие    | Игрок находится в комнате для игры                               |
| Постусловие    | Игрок выиграл                                                    |
