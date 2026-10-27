# survey_6read485-open

`survey_6read485` 的**版本检查公开仓库**。

本仓库**只放版本清单**，不含任何源码、配置、口令或采集数据。
客户端程序 `survey_6read485` 的「检查更新」功能读取
[`survey_6read485.json`](survey_6read485.json)，与本地版本号比较后提示是否有新版本。

## 文件

| 文件 | 说明 |
|---|---|
| `survey_6read485.json` | 版本清单：`version` / `date` / `notes` / `channel` / `platform` / `updated_at` |

程序按以下顺序尝试读取清单，取版本号最高者：

```
https://gitee.com/zpj100/survey_6read485-open/raw/master/survey_6read485.json
https://raw.giteeusercontent.com/zpj100/survey_6read485-open/raw/master/survey_6read485.json
https://fastly.jsdelivr.net/gh/zpj100/survey_6read485-open@master/survey_6read485.json
https://cdn.jsdelivr.net/gh/zpj100/survey_6read485-open@master/survey_6read485.json
https://gitee.com/api/v5/repos/zpj100/survey_6read485-open/releases/latest
https://raw.githubusercontent.com/zpj100/survey_6read485-open/master/survey_6read485.json
https://api.github.com/repos/zpj100/survey_6read485-open/releases/latest
```

## 发版流程

1. 私有仓库 `survey_6read485` 打 tag（`v1.7.0`）并把打包产物压缩包上传到 Releases；
2. 改本仓库 `survey_6read485.json` 的 `version`、`date`、`notes`、`updated_at`；
3. 提交并推送到 Gitee / GitHub（Gitee raw 即时生效，jsdelivr 有缓存，可能延迟数分钟）。

## 相关仓库

- 私有源码：<https://gitee.com/zpj100/survey_6read485>（Gitee）、<https://github.com/zpj100/survey_6read485>（GitHub）
