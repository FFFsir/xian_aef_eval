# xian_aef_eval

西安 AEF 评估项目——父仓库，通过 **git submodule** 持有两个子仓库：

| 子模块 | 仓库 | 内容 |
|--------|------|------|
| `download_scripts` | https://github.com/FFFsir/download_scripts | 基于 GEE 的遥感数据批量下载工具集（DynamicWorld + SatelliteEmbedding） |
| `evaluation_scripts` | https://github.com/FFFsir/evaluation_scripts | 卫星影像像素级 embedding 质量评估系统（KNN + Linear Probe） |

## 克隆（含子模块）

```bash
git clone --recurse-submodules https://github.com/FFFsir/xian_aef_eval.git
```

或已克隆后补拉子模块：

```bash
git submodule update --init --recursive
```

## 备注
- 各子仓库的详细使用文档见各自仓库的 `README.md`。
