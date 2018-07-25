* [Getting Started with TypeScript](#getting-started-with-typescript)
* [TypeScript Version](#typescript-version)

# Начало работы с TypeScript

TypeScript компилируется в JavaScript. JavaScript — это то, что вы на самом деле собираетесь выполнять (либо в браузере, либо на сервере). Таким образом, вам понадобится следующее:

* Компилятор TypeScript (доступен [в исходном коде](https://github.com/Microsoft/TypeScript/) или на [NPM](https://www.npmjs.com/package/typescript))
* Редактор для написания кода на TypeScript (вы можете использовать блокнот, если хотите, но я использую [vscode 🌹](https://code.visualstudio.com/) с [моим расширением](https://marketplace.visualstudio.com/items?itemName=basarat.god). Также [множество других редакторов кода и IDE поддерживают его]( https://github.com/Microsoft/TypeScript/wiki/TypeScript-Editor-Support))


## Версия TypeScript

Вместо использования *стабильной версии* компилятора TypeScript мы представим много нового в этой книге, которые пока не могут быть связаны с номером версии. Обычно я рекомендую использовать ночную версию, потому что **набор тестов компилятора со временем перехватывает больше багов**.

Вы можете установить его в командной строке как показано ниже:

```
npm install -g typescript@next
```

И теперь инструмент в командной строке `tsc` будет самой последней версии. Различные IDE также поддерживают его.

* Вы можете указать vscode использовать данную версию, создав файл `.vscode/settings.json` со следующим содержимым:

```json
{
  "typescript.tsdk": "./node_modules/typescript/lib"
}
```

## Получение исходного кода
Исходники кода этой книги доступны в [репозитории](https://github.com/basarat/typescript-book/tree/master/code), большинство примеров кода можно скопировать в vscode, и делать с ним всё, что угодно. Для примеров кода, которые нуждаются в дополнительной настройке (например, модули npm), мы дадим ссылку на пример кода до самого кода примера, например:

`this/will/be/the/link/to/the/code.ts`
```ts
// Это будет обсуждаемый код
```

С установкой для разработки закончено, теперь давайте перейдем к синтаксису TypeScript.
