# 开发2
Installing GitBook 3.2.3
执行gitbook serve的bug
Error: ENOENT: no such file or directory, stat 'C:\Users\Administrator\Desktop\htmlDemo\huangjunneng.github.io\_book\gitbook\gitbook-plugin-fontsettings\fontsettings.js'

解决方法：
cd ~/.gitbook/versions/版本/lib/output/website/copyPluginAssets.js

C:\Users\Administrator\AppData\Local\Temp\tmp-7788dPQ0lJGuOC6W\node_modules\gitbook\lib\output\website\copyPluginAssets.js

将112行的confirm改为false

```js
    return fs.copyDir(
        assetsFolder,
        assetOutputFolder,
        {
            deleteFirst: false,
            overwrite: true,
            confirm: false  //将此行改为false
        }
    );
```