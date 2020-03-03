ref -> https://kitigai.hatenablog.com/entry/2019/05/01/024341
https://kitigai.hatenablog.com/entry/2019/05/04/165522

xdebugの設定は下記

```
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Listen for XDebug",
            "type": "php",
            "request": "launch",
            "port": 9000,
            "pathMappings": {
                "/var/phpapp": "${workspaceRoot}/src"
            }
        }
    ]
}
```

# バックグラウンド実行
$ docker-compose up -d
--build
# コンテナの停止
$ docker-compose stop
# コンテナの停止＆削除 -> upで反映
$ docker-compose down