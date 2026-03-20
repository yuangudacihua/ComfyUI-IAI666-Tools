# ComfyUI-IAI666-Tools ✨
一个用于批量处理提示词、批量创建任务并逐一生成结果的 ComfyUI 自定义节点集合。

 感谢 B 站 UP 主 **AICoser 小姐姐** 原创节点和教学视频
---

## 🌟 功能特性
- **批量提示词节点**：支持批量加载/处理提示词，避免重复操作
- **任务队列管理**：创建多个生成任务，按顺序逐个执行
- **逐一生成结果**：执行时依次生成每张图片，便于调试和结果管理
- **前端界面集成**：提供简洁的 Web 界面，方便查看任务队列和进度


## 📦 安装方法

### 方法 1：通过 Git 安装（推荐）
1. 进入 ComfyUI 的 `custom_nodes` 目录：
   ```bash
   cd /path/to/ComfyUI/custom_nodes
   ```
2. 克隆本仓库：
   ```bash
   git clone https://github.com/yuangudacihua/ComfyUI-IAI666-Tools.git
   ```
3. 重启 ComfyUI，节点将自动加载。

### 方法 2：手动安装（夸克网盘下载）
1. 从夸克网盘下载节点文件：
   👉 [ComfyUI-IAI666-Tools 节点安装包](https://pan.quark.cn/s/66a228496ca8)
2. 解压后将文件夹重命名为 `ComfyUI-IAI666-Tools`
3. 放入 `ComfyUI/custom_nodes` 目录
4. 重启 ComfyUI

---

## 📚 教学视频（转载）
本节点的详细使用教程由 B 站 UP 主 **AICoser 小姐姐** 原创录制，感谢她的优质教学内容：
👉 [ComfyUI-IAI666-Tools 使用教程](https://www.bilibili.com/video/BV1kecszFEzx/?spm_id_from=333.788.videopod.sections&bvid=BV1YKkjBrEXf&vd_source=324ab94653925ab7a5c2ca6f5f9924d0)

---

## 🧩 节点列表

| 节点名称               | 功能描述                                   |
|------------------------|--------------------------------------------|
| Batch Load Images      | 批量加载本地图片文件                       |
| Prompt Queue Manager  | 管理提示词队列，支持批量添加/删除任务       |
| Batch Execution Node  | 按顺序执行队列中的任务，逐一生成结果        |

---

## 📝 使用示例

### 基础工作流
1. 在 ComfyUI 中添加 `Batch Load Images` 节点，节点搜索：666，选择需要处理的图片文件夹
2. 添加 `Prompt Queue Manager` 节点，输入批量提示词（每行一个提示词）
3. 连接 `Batch Load Images` → `Prompt Queue Manager` → 生成节点
4. 运行工作流，节点将自动按顺序生成所有结果

### 示例工作流截图
## 🖼️ 节点预览
![ComfyUI-IAI666-Tools 节点界面](https://github.com/yuangudacihua/ComfyUI-IAI666-Tools/blob/main/666-1.png)
![ComfyUI-IAI666-Tools 工作流界面](https://github.com/yuangudacihua/ComfyUI-IAI666-Tools/blob/main/666-3.png)

---

## ⚠️ 注意事项
- 首次运行节点时，Python 会自动生成 `__pycache__` 缓存目录，不影响功能
- 建议在 ComfyUI 日志中查看任务执行状态，便于排查问题
- 若节点未显示，请检查 ComfyUI 终端日志是否有报错信息


## 📄 许可证
本项目采用 MIT 许可证，详见 [LICENSE](LICENSE) 文件。

---

## 🙏 致谢
- 感谢 B 站 UP 主 **AICoser 小姐姐** 原创节点和教学视频

---

