### インストール
ローカル
```
npm install --save-dev shiftjis-server
yarn add -D shiftjis-server
```
グローバル
```
npm install -g shiftjis-server
yarn global add shiftjis-server
```

### 使い方 (ローカルインストール)
package.jsonに以下を追加 (./srcを監視)
```
  "scripts": {
    "server": "shiftjis-server -b -d ./src"
  },
```
実行
```
yarn server
npm run server
```

### 使い方 (グローバルインストール)
```
shiftjis-server -b -d ./src
```

### Usage for Command Line Application

```
Usage: shiftjis-server [options]

Options:

  -h, --help                     output usage information
  -V, --version                  output the version number
  -b, --browser                  Open in the browser automatically.
  -n, --hostname [hostname]      If -b flag is being used, this allows for custom hostnames. Defaults to localhost.
  -d, --dir [dir]                The directory to serve up. Defaults to current dir.
  -w, --watch-dir [watch-dir]    The directory to watch. Defaults the serving directory.
  -e, --exts [extensions]        Extensions separated by commas or pipes. Defaults to html,js,css.
  -p, --port [port]              The port to bind to. Can be set with PORT env variable as well. Defaults to 8080
  -s, --start-page [start-page]  Specify a start page. Defaults to index.html
  -f, --fallback [fallback]      Fallback to the start page when route is not found
  -v, --verbose [verbose]        Turning on logging on the server and client side. Defaults to false

```

参考ライブラリ
https://github.com/badcafe/reload-static