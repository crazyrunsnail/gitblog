# [Hello world!](https://github.com/crazyrunsnail/gitblog/issues/1)

这是我的第N次第一篇博客，花了30分钟把这个搭建成功了。

### Github操作
#### generate new token
名称 G_T,  选择了刚刚的repo, 权限选择的是Actions read and write, 无过期时间, 保存到 Notes
#### repo 中的操作
- Settings - Pages: Build and Deployment 选择 Github Actions
- Settings - Secrets  and Variables - Actions: 在 repository secrets 加上刚刚保存到 Notes 的 G_T
- Settings - Actions: 检查一下权限是 read and write
- Actions: 选择enable

### 本地操作
- clone 到项目到本地，把 `BACKUP` 删除掉所有的文件
- 修改 `main.py` MD_HEAD 可以获取 os.env
- 修改 `.github/workflows/generate_readme.ym`:  1. 在 `Generate new md` 增加 MD_HEAD 的 env
- 修改 `.github/workflows/generate_site.yml`: BASE_URL
- 修改 `config.toml` : 修改 base_url, even_title, even_menu


