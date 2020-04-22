### 新建用户

adduser admin // 新增用户
passwd admin  // 给用户设置密码
vim /etc/sudoers  // 找到 98 行，在 root 下面新增 admin ALL=(ALL)  ALL 给 admin 添加sudo 权限
su admin      // 切换用户

### 配置