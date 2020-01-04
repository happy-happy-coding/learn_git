# 极简Git使用手册
1. 在GitHub的Organization页面中打开你要clone的仓库，例如[本页面](https://github.com/happy-happy-coding/learn_git)。

2. 复制这个仓库的URL，例如`https://github.com/happy-happy-coding/learn_git`。

3. 在电脑上找一个地方来保存这个仓库。

   打开一个文件夹，然后按住 `SHIFT` 单击鼠标右键，选择 `在此处打开Powershell窗口` 菜单（这一步也可以使用任何你喜欢的命令行工具），进入命令行后输入：

   ```bash
   git clone <URL>
   ```

   例如，如果你要克隆本仓库，那么就把 `<URL>` 替换成 `https://github.com/happy-happy-coding/learn_git`：

   ```bash
   git clone https://github.com/happy-happy-coding/learn_git
   ```

   假设你执行这行指令时位于 `D:\` ，那么当指令执行完后，你的电脑上就会多出 `D:\learn_git` 目录。至此clone步骤结束。

4. 在仓库中编写代码、编辑文档。

5. 把你对仓库的更改提交到服务器上。

   这一步需要在命令行中执行三条指令，进入第3步中clone下来的仓库文件夹，并按之前的方式打开命令行，依次输入

   ```bash
   git add .
   git commit -m <message>
   git push
   ```

   即可将所有改动提交到服务器上。注意， `<message>` 字段是关于本次提交的描述信息，需要自行修改。
   
6. 别人在服务器上提交更改后，将更改同步到本地。

   同样在命令行中进入仓库文件夹，输入

   ```bash
   git pull
   ```

   就可以把自己本地的仓库同步为服务器上最新的状态。

# 更多Git资料

这份手册只是关于最常用的几条Git指令的**使用步骤**的介绍，关于这些指令背后的行为和更多指令的使用，可以参考Pro Git一书。