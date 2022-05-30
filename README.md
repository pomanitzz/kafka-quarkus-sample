Quarkus Kafka Quickstart
========================

This project illustrates how Quarkus applications can interact with Apache Kafka using MicroProfile Reactive Messaging.

## Start the application

The application is composed of two applications communicating through Kafka.
Interactions with Kafka is managed by MicroProfile Reactive Messaging.

They can be started in dev mode using:

```bash
mvn -f producer quarkus:dev
```

and in another terminal:

```bash
mvn -f processor quarkus:dev -Ddebug=5006
```

_NOTE_: Quarkus Dev Services starts a Kafka broker for you automatically.

Then, open your browser at `http://localhost:8080/quotes.html`.
You can send quote requests and observe received quotes.
