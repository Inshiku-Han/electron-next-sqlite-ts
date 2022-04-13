```sh
npm run pack-app
```

테스트용 앱 빌드

```sh
npm run dist
```

찐 앱 빌드

```sh
npm run rebuild
```

이거 안하면 better-sqlite3 안돌아감

rendererProcess에서 mainProcess로 송, 수신 가능

```js
ipcRenderer.send("banana", { a: 1 });
```

```js
ipcMain.on("banana", (_, ...args) => {
  console.log(args); // [{ a: 1}]
});
```
