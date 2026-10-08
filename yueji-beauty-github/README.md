# 悦己美学 · 美业小程序项目

根据需求讨论整理的单门店综合美业项目。**当前代码是可运行的网页交互原型，不是已经完成的微信原生小程序。**

## 已实现

- 首页、活动、项目分类、价格与项目详情。
- 服务人员、日期、时间选择，预约提交、冲突校验及取消。
- 普通会员中心、模拟储值、余额与流水。
- 模拟消费积分、积分兑换、优惠券。
- 门店信息与客服、导航的待配置说明。

数据只存在当前页面内存中，刷新即清空；不产生真实预约、充值或消费。客服电话、门店地址与店名均为占位内容。

## 运行

直接打开 `index.html` 即可体验。也可以在项目目录运行：

```sh
python -m http.server 8080
```

随后访问 `http://localhost:8080`。无依赖安装、无构建步骤。

## 目录

```text
index.html          页面入口
styles.css          响应式样式
app.js              项目数据与交互逻辑
docs/requirements.md 已确认需求、业务规则与待开发范围
.gitignore          排除本地环境和密钥文件
```

## 上传 GitHub

1. 新建一个空仓库，建议初期设为 Private。
2. 解压代码包，进入 `yueji-beauty-github` 文件夹。
3. 在 GitHub 仓库选择 Add file → Upload files，把此文件夹内的文件和 docs 文件夹上传，提交即可。上传解压后的源码，不要只上传 ZIP。

也可在本地使用 Git：

```sh
git init
git add .
git commit -m "Add beauty booking prototype and requirements"
git branch -M main
git remote add origin <替换为你的GitHub仓库地址>
git push -u origin main
```

## 正式微信版的状态

尚未实现微信登录、后端持久化、店家后台、微信支付、退款、真实积分和储值记账。不要将原型用来收取真实款项。完整范围见 `docs/requirements.md`。

原演示页面中的第三方门店照片未纳入此代码包；请使用自己拥有使用权的门店照片。
