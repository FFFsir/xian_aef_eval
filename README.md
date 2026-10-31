# xian_aef_eval

西安 AEF 评估项目——父仓库，通过 **git submodule** 持有三个子仓库：

| 子模块 | 仓库 | 内容 |
|--------|------|------|
| `download_scripts` | https://github.com/FFFsir/download_scripts | 基于 GEE 的遥感数据批量下载工具集（DynamicWorld + SatelliteEmbedding） |
| `evaluation_scripts` | https://github.com/FFFsir/evaluation_scripts | 卫星影像像素级 embedding 质量评估系统（KNN + Linear Probe） |
| `change_detection_scripts` | https://github.com/FFFsir/change_detection_scripts | 基于 AEF 嵌入的无监督变化检测 WebUI（NiceGUI，单文件应用） |

## 克隆（含子模块）

```bash
git clone --recurse-submodules https://github.com/FFFsir/xian_aef_eval.git
```

或已克隆后补拉子模块：

```bash
git submodule update --init --recursive
```

## 更新子模块

```bash
git submodule update --remote --merge
```

## 备注

- 三个子仓库均为 **public**，可直接克隆与浏览。
- 各子仓库的详细使用文档见各自仓库的 `README.md`：
  - `download_scripts`：[docs/](./download_scripts/docs/) 下的下载教程与架构指南
  - `evaluation_scripts`：仓库 `README.md`
  - `change_detection_scripts`：[docs/webui-user-guide.md](./change_detection_scripts/docs/webui-user-guide.md)（含数据目录结构要求）
- `change_detection_scripts` 的 `data/` 目录（约 2.2 GB 数据包）不纳入版本控制，需按使用说明书第 2.4 节准备本地数据包。
