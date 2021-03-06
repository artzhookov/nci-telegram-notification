# nci-telegram-notification
[![Build Status](https://travis-ci.org/node-ci/nci-telegram-notification.svg?branch=master)](https://travis-ci.org/node-ci/nci-telegram-notification)

Telegram notification plugin for [nci](https://github.com/node-ci/nci)

## Installation

```sh
npm install nci-telegram-notification
```

## Usage

Register telegram bot, just start conversation with `@BotFather`.
Add this plugin to the `plugins` section at server config, set
parameters for telegram bot at `notify.telegram`
```yml
plugins:
    - nci-telegram-notification

notify:
    telegram:
        token: 123:xyz

```
after that you can set telegram notification at project config
```yml
notify:
    on: [done, change, error]
    to:
        telegram:
            - 1111
```

## License

[The MIT License](https://raw.githubusercontent.com/fleg/nci-telegram-notification/master/LICENSE)
