# java-wechaty-getting-started
[![Powered by Wechaty](https://img.shields.io/badge/Powered%20By-Wechaty-green.svg)](https://github.com/chatie/wechaty)
[![Wechaty开源激励计划](https://img.shields.io/badge/Wechaty-开源激励计划-green.svg)](https://github.com/juzibot/Welcome/wiki/Everything-about-Wechaty)

[![Java CI with Maven](https://github.com/wechaty/java-wechaty-getting-started/workflows/Java%20CI%20with%20Maven/badge.svg)](https://github.com/wechaty/java-wechaty-getting-started/actions?query=workflow%3A%22Java+CI+with+Maven%22)

Java Wechaty Starter Project Template that Works Out-of-the-Box

![Java Wechaty](https://wechaty.github.io/java-wechaty/images/java-wechaty.png)

## Connecting Chatbots

[![Powered by Wechaty](https://img.shields.io/badge/Powered%20By-Wechaty-brightgreen.svg)](https://github.com/Wechaty/wechaty)
[![Java Version](https://img.shields.io/maven-central/v/io.github.wechaty/wechaty?label=Java)](https://mvnrepository.com/artifact/io.github.wechaty/wechaty)

Wechaty is a RPA SDK for Wechat **Individual** Account that can help you create a chatbot in 6 lines of Java.

## The World's Shortest Java ChatBot: 6 lines of Code

```java
class Bot{
  public static void main(String args[]){
    bot = Wechaty.instance()
      .on('scan', (qrcode, status string) -> System.out.println('Scan QR Code to login: %s\nhttps://api.qrserver.com/v1/create-qr-code/?data=%s', status, encodeURIComponent(qrcode)))
      .on('login', user -> System.out.println('User %s logined', user))
      .on('message', message -> System.out.println('Message: %s', message))
      .start();
  }
}
```

## Usage

### Install

```sh
# Install Maven
apt install maven

make install
```

### Run

```sh
make bot
```

## Wechaty Getting Started in Multiple Languages

- [TypeScript Wechaty Getting Started](https://github.com/wechaty/wechaty-getting-started)
- [Python Wechaty Getting Started](https://github.com/wechaty/python-wechaty-getting-started)
- [Java Wechaty Getting Started](https://github.com/wechaty/java-wechaty-getting-started)
- [Go Wechaty Getting Started](https://github.com/wechaty/go-wechaty-getting-started)

## Copyright & License

- Code & Docs © 2020-now Wechaty <https://github.com/wechaty>
- Code released under the Apache-2.0 License
- Docs released under Creative Commons
