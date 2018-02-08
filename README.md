### ReactJS_HW
#Homework on React


## Домашнее задание #1

* Сделать header приложения, в нем лого и будущая навигация.
* Создать галлерею карточек кинофильмов.
* Создать форму для будущего добавления кинофильмов.
* Пока что функционала нет, просто готовим скелет из компонентов.


## Домашнее задание #2

* В текущем приложении добавить возможность удаления карточек из галлереи по
  нажатию на кнопку **Delete**.
* Реализовать возможность добавлять новые карточки используя форму.

### **Бонус:**

* Запретить создание карточки кинофильма если поля **Title** и **Description**
  не заполнены. Выводить простой **alert** с оповещением о незаполненых полях.
* Сделать добавление категорий кинофильма через чекбоксы формы.


## Домашнее задание #3

* Реализовать поиск кинофильмов через API, по имени.
* По прибытию данных от API, по полученой информации, должен произойти рендер
  карточек в галлерее.
* При первой загрузке страницы должны автоматически приходить и отображаться
  популярные кинофильмы.

### **Бонус**

* Добавить панель **Watchlist**, в которую будут добавляться/удаляться те
  карточки, которые были отмечены пользователем.
* Реализовать возможность добавлять карточки в **Watchlist** при помощи кнопки +
  на карточке кинофильма в галлерее. Карточки добавляются в **watchlist**,
  массив карточек "любимых" фильмов.
* В **Watchlist** не должно быть дубликатов. Если добавляемый кинофильм уже есть
  в Watchlist, не добавлять.
* Реализовать возможность удаления карточки из **Watchlist** при помощи кнопки -
  на карточке в списке **Watchlist**.

### **Бонус бонус**

* Сохранить список карточек **watchlist** в **localStorage**, чтобы после
  перезагрузки страницы пользователь все еще видел выбраные карточки.
* Создать 3 кнопки для поиска кинофильмов по категориям: popular, top rated и
  upcoming.

#### API

* Api Endpoint: https://api.themoviedb.org/3/
* [Документация по поиску кинофильма по имени](https://developers.themoviedb.org/3/search/search-movies)
* [Документация по категориям поиска](https://developers.themoviedb.org/3/tv)

### [Пример рабочей версии](https://axzerk.github.io/react-minicourse/hw-03/)

## Домашнее задание #4

* Создать базовый раутинг: домашняя страница (home), страница поиска кинофильмов
  (movies), страница информации (about).
* При клике по ссылке главной навигации, должен происходить переход по
  соответствующим раутам.
* Хедер с навигацией не входят в раутинг и рендерятся всегда на старте.
* Домашняя страница должна "открываться" по умолчанию при посещении приложения.
  На ней должен быть текст с приветствием и 2 ссылки, одна на страницу
  кинофильмов, вторая на страницу информации.

### **Бонус:**

* На странице About, сделать subroutes, простое меню которое содержит несколько
  ссылок: team, stack, career. При клике по ним происходит добавление пути в
  текущий раут, к примеру about/team.
* В зависимоти от того какой subroute выбран на странице about, под меню
  рендерится соответствующий компонент.
* В сабрауте about/team рендерится компонент содержащий список членов команды.
  При клике по имени в списке, рендерится компонент карточки члена команды. Это
  делается с помощью использования history, поля match.params. В конец url
  строки добавляется id члена команды и, компонент карточки с информацией о нем,
  использует match.params.параметр для отображения информации.

### [Пример рабочей версии](https://axzerk.github.io/react-minicourse/hw-04/)

