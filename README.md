По вопросам обращайся в телеграмм @ZenkoWu

Для проверки работы релизного воркфлоу нужно пушить следующий по счету тег - предыдущим был v3, тебе нужно запушить v4, затем v5 и тд.
Предыдущие теги можно посмотреть в репозитории.

В этом репозитории находится пример приложения с тестами:

- [e2e тесты](e2e/example.spec.ts)
- [unit тесты](src/example.test.tsx)

Для запуска примеров необходимо установить [NodeJS](https://nodejs.org/en/download/) 16 или выше.

Как запустить:

```sh
# установить зависимости
npm ci

# запустить приложение
npm start
```

Для линтинга коммитов необходимо установить:

```sh
npm install @commitlint/cli
npm install @commitlint/config-conventional
npm install husky 
npx husky install

```
Как запустить все тесты:

```sh
npm run test-ci
```
Как запустить e2e тесты:

```sh
# скачать браузеры
npx playwright install

# запустить тесты
npm run e2e
```

Как запустить модульные тесты:

```sh
npm test
```
