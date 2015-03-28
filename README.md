# Chatty

Необходимо разработать небольшой чат с одной комнатой.
API:
``` erlang
  start/0 - запуск сервера.
  stop/0  - останов сервера.

  connect(Node) - подключение к узлу Node как к серверу.
  disconnect(Node) - отключение от узда Node.

  send(Message, Node) - отправка сообщения Message на сервер Node. Ожидаение ответа от сервера не более трех секунд.
```

Для приложения необходимо реализовать два внутренних процесса - серверный и клиентский. Серверный процесс осуществляет массовую рассылку сообщений между подключившимися клиентами, а клиентский - печатает сообщения от сервера.
