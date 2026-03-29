# [Hello world!](https://github.com/crazyrunsnail/gitblog/issues/1)

这是我的第N次第一篇博客，花了30分钟把这个搭建成功了。

选择yihong的gitblog作为我的个人博客模版很简单，一直在使用running_page,  gitblog又有一点hack的味道，和之前搭的静态个人博客不一样，gitblog 是先在 issues 写然后再备份到 repo， 如果真的是挑毛病，那就 Github 没有原生支持 issues 只能限制本人新建。

还不知道将来自己的博客要写些什么，但AI时代，独立思考和独立写作显得更加的重要。作为一个开发，应该是技术为主输出。现在只定了两label: Top 和 技术文章

我知道博客模版向来不是难点，难的是持续且稳定地输出，在是在AI时代，这显得更难。在之前想写一个技术文章，心里会想“这肯定早就有写过了，写了没什么用”，现在会多一个理由“这个查一下AI就行了”

我也同样有这样的困惑，我也不清楚，在这段时间还是花了一点点时间来搭建，可能还是有一些变化在我自身上发生

如果将博客不是定位为向外输出，而是向内输出或者“证明自己不是AI”，是一面镜子，那么这样写博客可能会轻松处在一些

---
我是怎么搭建这个博客的？

fork 一份 yihong 的 gitblog 后，主要是 `Github操作` 和 `本地操作`

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
- 修改 `main.py`: 将 MD_HEAD 改成是自己的
- 修改 `.github/workflows/generate_site.yml`: BASE_URL
- 修改 `config.toml` : 修改 base_url, even_title, even_menu
- push到远程



