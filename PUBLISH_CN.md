# SFGFusion 网页发布说明

## 方案一：先发布到你自己的 GitHub Pages（最简单）

1. 登录 GitHub，点击右上角 `+` → `New repository`。
2. Repository name 填：`SFGFusion`。
3. 建议选择 `Public`，然后点击 `Create repository`。
4. 把本文件夹里的所有内容上传到仓库根目录，确保 `index.html` 位于仓库最外层。
5. 进入仓库：`Settings` → `Pages`。
6. `Build and deployment` 中：
   - Source：`Deploy from a branch`
   - Branch：`main`
   - Folder：`/(root)`
   - 点击 `Save`
7. 等待 1–3 分钟，刷新 Pages 设置页，会看到发布地址：
   `https://你的GitHub用户名.github.io/SFGFusion/`

## 方案二：发布成和 DogMo 一样的 PIE Lab 地址

DogMo 的源代码仓库是 `BIT-PIE/DogMo`，网页地址是 `https://pie-lab.cn/DogMo/`。因此要得到完全一致的域名形式，建议按实验室现有项目页发布机制操作：

1. 在 `BIT-PIE` 组织下新建 `SFGFusion` 仓库，或者请维护 PIE Lab 网站的同学/老师新建。
2. 将本文件夹完整上传到该仓库，`index.html` 放在网页发布分支的根目录。
3. 参考 `BIT-PIE/DogMo` 当前使用的 `Page` 分支/站点映射方式配置发布。
4. 如果 PIE Lab 主站由服务器/Nginx 做子目录映射，需要管理员把 `SFGFusion` 静态目录映射到 `/SFGFusion/`。
5. 最终目标地址：`https://pie-lab.cn/SFGFusion/`。

注意：仅在你自己的 GitHub 中开启 Pages，默认只能得到 `github.io` 地址；要使用 `pie-lab.cn/SFGFusion/`，必须有 PIE Lab 域名或主站仓库/服务器的管理权限。

## 发布前建议做两项修改

1. 代码公开后，把首页的 `Code · coming soon` 改成真实 GitHub 代码仓库链接。
2. 当前论文图片直接引用 arXiv 公共图片地址。网页可以直接发布；如果希望长期稳定、完全独立，建议把论文图片下载到 `static/images/`，再把 `index.html` 中的远程 URL 改成本地相对路径。
