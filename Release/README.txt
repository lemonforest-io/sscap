SSCap是一个Windows下C++版的Shadowsocks客户端. 相比其它的客户端更稳定更快速,不会出现其它版本中常现的接收数据错误.

2017.04.14 3.7
1, 修改IP显示的一个BUG.

2017.04.13 3.6
1, 主界面中加入节点所在区域的查寻显示.
2, 改正退出提示文字错误.
3, 改正删除所有节点后,重启又回来了的问题.
4, 支持某些网站生成的json格式.
5, 修正启用系统代理后，PAC模式无法打开海外网站的问题 
6, 解决启动程序时产生端口冲突则有可能导至浏览器无法使用
7, 增加PING节点功能

2016.12.10 3.5
1, 将Privoxy封装成DLL, 从而不再需要带着Privoxy进程以及一堆Templates文件.
2, 增加本地Http代理
3, 解决CURL请求时提示:"No authentication method was acceptable."的问题.
4, PAC模式从"黑名单"机制改为"自动跳过所有中国网站"
5, 节点实时速度统计改进. 
6, 加入DNS解析的缓存机制, 一定程度上提升连接时解析速度.
7, 增强JSON解析的兼容性. 能解析某些错误的JSON格式.

2016.08.24 3.3
1, 修复某些情况下无法编辑节点备注的BUG. 
2, 修复某些情况下编辑节点时导至程序崩溃的BUG.
3, 增加拷贝到节点明文信息
4, 节点备注信息可以更长.

2016.08.08 3.2
1, 修改默认启用系统代理的逻辑.用户手动禁用系统代理后不再恢复之前保存的系统代理.
2, 兼容新的SS链接格式.
3, 其它小BUG修改.

2016.04.21 3.1
1, 新增支持chacha20-ietf加密
2, 支持通过热捷键截图二维码来添加节点( 设置中启用 )
3, 程序启动时不再加载之前的节点延迟及速度信息
4, 修改节点排序中上传下载流量排序错误的问题.

2016.04.02 3.0
1, 系统托图标弹出菜单中的关于点击没有响应.
2, 通过JSON格式添加节点时导至程序出错退出.
3, 应网友要求:增加可以设置测试节点用的URL(在设置中修改)
4, 应网友要求:启动时记忆IE系统代理的配置并在退出程序时恢复之前的配置.
5, 能显示新版本更新的内容

2016.03.30 2.9
1, 主界面中删除一些节点再添加一些节点后在托盘弹出菜单中就不能正常的切换节点了.
2, 启动多个SSCap进程时,后启动的进程会导至之前启动的进程无法工作.
3, 启用服务器均衡同时有节点被禁用则可能导至程序出错退出.

2016.03.24 2.8
1, 应网友要求, 增加切换点时自动断开前节点所有连接的功能(在设置中启用)

2016.03.16 2.7
1, 未选中节点时不能测试所有节点的问题.
2, 优化节点测试窗口.

2016.03.14 2.6
1, 优化节点出错重连机制.

2016.03.11 2.3
1, 节点列表经排序后修改节点信息错乱(修改到了其它节点的信息)
2, 重复测试节点的问题.( 测试节点时会将之前测试过的重复测试一次)

2016.03.10 2.2
1, 节点排序时未正确按数据大小排序的问题.
2, 因为节点密码较长可能导至程序在使用中出错退出的BUG.
3, 节点添加备注后无法删除备注信息.
4, 修改在高DPI下程序界面错乱的问题.
5, 支持从未BASE64的明文SS LINK加入节点.
6, 增加清除所有节点流量信息的功能.
7, 修改添加节点时的JSON格式, 兼容其它版本的JSON格式.

2016.03.09 2.1
1, 修正在最新版的libev服务器端下有可能打不开网站的问题.
2, 增加测试所有节点的功能(主界面右键菜单中).
3, 修正在系统托盘菜单中切换节点后托盘图标提示的当前节点仍未改变的BUG.
4, 修正主界面中通过右键菜单禁用一个节点后再启用节点无法启用的BUG.
5, 修正被禁用的节点仍然可以被使用的问题.
6, 修正被禁用的节点在系统托盘右键菜单中仍然可以使用的问题.
7, 修正主界面中的节点被排序后更新状态时会错乱的问题.

2016.03.06 1.9
1, 修正WIN 10系统下 PAC模式下不能正确代理网站的问题.
2, 增加结束某个节点的所有连接的功能. ( 切换代理后希望将之前代理的连接全断开)
3, 主界面中SS节点信息动态更新时加以颜色区分.
4, 修正按扭禁止时状态不对的BUG
5, 升级时可以选择下载源.

2016.01.03 1.8
1, 修改主界面连接数不会变动的BUG.
2, 系统托盘菜单添加: 切换全局模式/PAC模式.
3, 系统托盘菜单添加: 更新线上PAC文件功能.
4, 系统托盘菜单添加: 编辑本地PAC文件功能.
5, 加入功能: 增加用户PAC文件, 可以实时将希望通过代理的域名添加到用户PAC文件并立即生效.
6, 一些小bug修改

2015.12.24 1.7
/////////////////////////////////////////////////////
1, 二维码截图方式修改.
2, 修正SOCKS 5的帐号密码的验证时的BUG.
3, 修正系统代理PAC模式下的BUG: SSCAP绑定了1080外的其它端口,但是系统代理中PAC地址端口仍然是1080.
4, 切换当前代理后,系统托盘中的当前代理信息不会改变.
5, 修改本地SOCKS 5代理端口后,系统设置中的代理端口不会改变.
6, 修改本地SOCKS 5代理端口后,privoxy中转端口未修改.

2015.12.15 1.6
/////////////////////////////////////////////////////
1, 应网友要求: 增加启动时最小化到系统托盘功能. (请在系统设置中启用此功能)

2015.12.12 1.5
/////////////////////////////////////////////////////
1, 增加端口被占用时自动搜索端口功能.

2015.12.08 1.4
/////////////////////////////////////////////////////
1, 增加'复制到'功能,可以将一个SS节点复制到二维码/JSON/SS链接
2, 可以手动修改本地SOCKS监听端口.
3, 可以通过将SSCap拷贝到新目录来实现运行多份SSCap实例.

2015.11.30 1.3
/////////////////////////////////////////////////////
1, 修正在rc4-md5,salsa20兩種加密方式下的嚴重BUG導至無法工作.
2, 修改系統代理的工作方式.

2015.11.28 1.2
/////////////////////////////////////////////////////
first issue, Key Features:
1, Support aes-256-cfb/aes-192-cfb/aes-128-cfb,md5,rc-md5,chacha20,chacha20-ietf,salsa20 encryption.
2, Test shadowsocks node in sscap
3, Show speed and traffic of every ss node.
4, support from win xp to win 10 windows os.