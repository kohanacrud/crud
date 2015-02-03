# KohanaCrud v1.0
Module for Kohana framework that will allow for a few lines of code to deploy a full-fledged CRUD with a nice interface.

Модуль для Kohana 3.2.x который позволит быстро всего в несколько строк кода развернуть полноценный CRUD c красивым интерфейсом.
Обладает большим набором методов и хуков для гибкой настройки и в 90% случаев удовлетворит все ваши пожелания. 
Призван освободить разработчика от решений тривиальных задач.

v.Kohana 3.2.x

Quick Start

      class Controller_Test extends Controller {

      public function action_index() {
          $this->response->body(self::asd()->render());
      }


      public static  function asd () {
          $crud = new Cruds;
          $crud->load_table('table');
      }
      }

Для начала роботы требуется базовые настройки. Это создание объекта класса и определение таблицы в нашем случае table. Создание объекта класса должно находится в статическом методе, название произвольное. И непосредственно вывод self::asd()->render(). См. Пример выше.
