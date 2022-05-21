# miniprogram-json-schema

Json Schema for MiniProgram config files Validation and IntelliSense.
小程序配置文件 json 验证和自动提示 schema

[![代码自动提示](https://user-images.githubusercontent.com/6290356/57195589-154ac300-6f87-11e9-8933-83d6784d5c2d.gif)](https://github.com/NewFuture/miniprogram-json-schema/issues/4)

## 使用说明

1. `package.json` 添加 `devDependencies` `"miniprogram-json-schema": "https://github.com/sssylvan/miniprogram-json-schema.git#master"`
1. `npm install`
1. 关联文件 .vscode/settings.json

```json
{
  "json.schemas": [
    {
      "fileMatch": ["app.json"],
      "url": "./node_modules/miniprogram-json-schema/schema/app.json"
    },
    {
      "fileMatch": ["project.config.json"],
      "url": "./node_modules/miniprogram-json-schema/schema/project.config.json"
    },
    {
      "fileMatch": ["sitemap.json"],
      "url": "./node_modules/miniprogram-json-schema/schema/sitemap.json"
    },
    {
      "fileMatch": ["src/app/pages/**/*.json"],
      "url": "./node_modules/miniprogram-json-schema/schema/page.json"
    },
    {
      "fileMatch": ["src/components/**/*.json"],
      "url": "./node_modules/miniprogram-json-schema/schema/component.json"
    }
  ]
}
```

## References

- <https://developers.weixin.qq.com/miniprogram/dev/framework/config.html>
- <https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/app.html>
- <https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/page.html>
- <https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/sitemap.html>
- <https://developers.weixin.qq.com/miniprogram/dev/devtools/projectconfig.html>

- <https://github.com/qiu8310/minapp> (初始定义 <https://github.com/qiu8310/minapp/tree/master/schema>)
- <https://www.jsonschemavalidator.net/>
- <http://yapi.demo.qunar.com/editor/>
