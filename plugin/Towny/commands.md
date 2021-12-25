# 命令

### ```/towny``` 城镇指令
* （无子命令） - 展示基本的城镇指令.&#x20;
* ? – 展示更多城镇指令.&#x20;
* map – 展示城镇地图.&#x20;
* prices – 展示城镇税收和维护费用.&#x20;
* time –展示到下一天的时间 (征收税收/维持费.)&#x20;
* top 排行&#x20;
  * residents {all/town/nation} – 列出所有/城镇/国家的居民列表.&#x20;
  * land {all/resident/town} – 展出拥有土地最多的人.&#x20;
* spy – 管理员指令,窥视所有聊天频道的信息&#x20;
* tree – 显示大量内容.只能在后台使用&#x20;
* universe – 显示所有城镇的数据, 居民/城镇/国家/世界 已声明的城镇区块计数.&#x20;
* v – 显示插件版本.&#x20;
* war -- 战争&#x20;
  * stats -- 数据&#x20;
  * scores -- 纪录&#x20;
  * hud -- 开关给予玩家战争时的土地信息的HUD.&#x20;
  * participants {page #} -– 列出参战者名单.
### ```/plot``` 地皮指令
* – 展示 /plot 指令.
* claim – 居民用来购买出售的土地的指令.
  * auto – 居民用来自动购买附近出售中的土地的指令.
* unclaim – 居民放弃自己的土地的指令.
  * circle/rect – 自动放弃区域内的自己的土地.(圆形/矩形 下同)
  * {# (以当前位置半径)} – 放弃土地的半径.
* {forsale/fs} – 出售一块土地.
  * circle/rect – 设置选区形状.
  * {# (以当前位置半径)} – 出售土地的半径.
  * $ – 土地价格.
  * circle/rect – 设置选区形状.
  * {# (以当前位置半径)} – 出售土地的半径.
* {notforsale/nfs} – 设置土地无法出售.
  * circle/rect – 设置选区形状.
  * {# (以当前位置半径)} – 设置无法出售的土地的半径.
* perm – 展示玩家所在区块的权限.
* perm hud – 开关显示更多土地权限信息的hud计分版.
* set
* reset – 把其他类型的土地重置为普通的土地.
* shop – 设置土地为商店.
* embassy – 设置地皮为大使馆.
* arena – 设置地皮为竞技场.
* wilds – 设置地皮为荒野.
* inn – 设置地皮为旅店.
* jail – 设置地皮为监狱.
* name – 允许城镇或地主重命名地名, 覆盖默认的~Unknowned.个人土地会显示地主名和地名.
* perm - 编辑土地权限
  * {on/off} – 启用/关闭权限限制.
  * {resident/ally/outsider} {on/off} -开关 居民/盟友/外来者 的权限
  * {build/destroy/switch/itemuse} {on/off} -开关 建筑/破坏/开关/物品使用 权限
  * {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off} -开关 居民/盟友/外来者 的 建筑/破坏/开关/物品使用 权限
* reset – 重置地皮权限为 /town 或 /resident 上的默认权限 (取决于是地主还是他人使用该指令)
* toggle
* fire – 开关你所站土地的火势蔓延.
* pvp – 开关你所站土地的PVP.
* explosion – 开关你所站土地的爆炸.
* mob – 开关你所站土地的怪物生成.
* clear – 回溯土地归于原生, 只会回溯配置内指定类型的方块.
### ```/town``` 城镇指令
缩写: ```/t```
* – 展示玩家所在的城镇信息.
* ? – 展示可用的/town指令.
* {城镇名} – 显示某个城镇的信息.
* here – 显示你所站在的那个城镇的信息.
* leave – 离开城镇.
* list {page #} – 列出城镇列表.
* online – 显示你所在城镇的在线玩家.
* plots {城镇名} – 展示城镇内的土地及其种类和税收.
* new
  * {城镇名} – 创建新城镇.
  * {城镇名} {城主} – 创建城镇(管理员指令).
* add {居民} .. {居民} – 邀请玩家到你的城镇内(城主指令).
* kick {居民} .. {居民} – 把一个玩家踢出你的城镇(城主指令).
* spawn – 传送到城镇出生点.
* spawn {城镇名} – 传送你到其他城镇的出生点.
* claim – 声明你所在的区块为城镇所有(管理员/助手指令).
* outpost – 为你的城镇建立前哨.
* {# (以当前位置为半径)} – 声明附近的区块为你的城镇所管辖.
* auto – 尽可能多地自动声明你附件的区块为你的城镇所管辖.
* unclaim – 放弃管辖当前区块.
  * all – 放弃管辖所有城镇区块(城主指令).
  * {# (以当前位置为半径)} – 放弃附近的区块为你的城镇所管辖.
  * outpost – 用于放弃前哨.
* withdraw {$} – 从城镇银行内取钱.
* deposit {$} – 捐钱给城镇.
* buy
  * bonus {amount} – 购买可用城镇区块上限.
* delete {town name} – 删除城镇及其数据(管理员/城主指令)(解散城镇使其分崩离析).
* outlawlist {城镇名} – 列出城镇放逐者列表.（92版本才有）
* outlaw {add/remove} {name} –从城镇放逐者列表中添加或移除玩家（92版本才有）
* outpost
  * {# ( #相当于相应的前哨编号)} – 传送到一个前哨.
  * {list} – 列出你的城镇前哨.
* ranklist – 展示居民头衔.
* rank {add|remove} {玩家名} {头衔名} – 给予或移除一个居民的头衔.
* reslist {城镇名} – 查看一个城镇内的所有居民.
* say {msg} – 向城镇成员广播信息.
* set
  * board {信息} – 设置公告栏信息(居民在每次登录时会看到的信息).
  * mayor {居民} – 将你的城主之位传给下一代(城主指令).
  * homeblock – 设置城镇中心区块(传送点).
  * spawn – 设置城镇传送点, 必须在城镇中心区块内.
  * name {名称} – 改变你的城镇名.
  * outpost – 设置一个城镇区块为前哨.
  * jail – 重置监狱的传送点到你所在的位置.
  * perm - 城镇权限设置
    * {on/off} – 开关
  * {resident/ally/outsider} {on/off} - 开关 居民/盟友/外来者 权限
  * {build/destroy/switch/itemuse} {on/off} - 开启或关闭 建筑/破坏/开关/物品使用 权限
  * {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off} -  开关 居民/盟友/外来者的 建筑/破坏/开关/物品使用 权限
  * reset –这个指令将会重置城镇内所有的地皮权限为默认地皮设置.
* tag {最多4个标签} – 设置城镇标签(可改变聊天的格式).
* clear – 清除城镇标签.
* taxes {$} – 设置固定的每日税收. 也可以设置为税收率.
* plottax {$} – 设置土地税, 按照居民拥有的土地数来收税.
* plotprice {$} – 设置城镇的默认土地价格.
* shopprice {$} – 设置默认的商店地皮价格.
* shoptax {$} – 设置商店地皮税, 按照拥有的商店地皮来收税.
* embassyprice {$} – 设置默认大使馆地皮价格.
* embassytax {$} – 设置大使馆地皮税, 按照拥有的大使馆地皮来收税.
* toggle
  * explosion – 开关城镇内的爆炸.
  * fire – 开关城镇内的火势蔓延.
  * mobs – 开关城镇内的敌对怪物生成.
  * public – 对外人是否开启城镇传送点.
  * pvp – 开关城镇内的PVP.
  * taxpercent – 开关按税率收税.
  * open – 开放/关闭公开城镇.
  * jail {number} {居民名} – 把你城镇内的居民羁押到监狱内. 再次输入指令释放囚犯.
* join {城镇名} – 加入公开的城镇.
### ```/resident``` 个人指令
缩写: ```/p```, ```/res```
* （无子命令） - 你的状态
* ```[玩家名]``` - 目标玩家状态
* ```list``` - 列出所有玩家
* ```tax``` - 查看税收
* ```jail``` - 监狱状态
* ```toggle``` - [模式]...[模式]
* ```set mode``` - 城镇模式
  * ```clear``` - 清除模式
  * ```map``` - 在你走到另一个城镇区块时显示城镇地图
  * ```townclaim``` - 声明你走过的区块(荒野)
  * ```townunclaim``` - 放弃你走过的区块的土地(城镇区块)
  * ```tc``` - 默认进入城镇聊天频道
  * ```nc``` - 默认进入国家聊天频道
* ```friend [add/remove] [玩家名]``` - 添加/移除 好友
* ```friend [add+/remove+] [玩家名]``` - 精确名称
* ```spawn``` 传送到个人传送点
### ```/nation``` 国家指令
缩写: ```/n```, ```/nat```
* – 显示玩家所在国家的情况.
* ? – 显示 /nation 指令.
* list {页码} – 列出所有国家.
* online – 显示在线的国人.
* {国家名} – 显示某个国家的信息.
* leave – 从祖国的怀抱中挣脱(城主指令).
* withdraw {$} – 从国库中取钱(国王指令).
* deposit {$} – 捐钱给国家.
  * new
  * {国家名} – 建国.
  * {国家名} {国都} – 创建新的国家并设置某个城镇为国都(管理员指令).
* rank – 设置国家内的助手/自定义头衔.
* add {城镇名} .. {城镇名} – 邀请一个城镇加入你的国家.
* kick {城镇名} .. {城镇名} – 把一个城镇踢出你的国家.
* delete {国家名} – 灭国 (国王指令).
* ally
* add {国家名} .. {国家名} – 把一个国家视为盟国.
* remove {国家名} .. {国家名} – 不再把一个国家视为盟国.
* enemy
* add {国家名} .. {国家名} – 把一个国家视为敌国.
* remove {国家名} .. {国家名} – 不再把一个国家视为敌国.
* rank {add|remove} {玩家名} {头衔名} – 给予一个玩家国家头衔.
* say {msg} – 广播信息给在线的国民.
  * set
  * king {居民} – 把一个玩家加冕为王.
  * captial {城镇名} – 设置国都.
  * taxes {$} – 设置国税.
  * name {国名} – 设置国家名.
  * title {名称} {头衔内容} –  给国家添加头衔(国王指令).
  * surname {名称} {surnamegoeshere} – 给国民冠以姓氏(国王指令).
  * tag {最多4个标签} – 设置国家标签.
  * clear – 清除国家标签.
* toggle
  * neutral – 是否设置你的国家在战争期间每日付费来保持中立.
### /townyadmin 管理员指令
缩写: /ta
* – 显示内存, 线程, 战争状态, 生命恢复设置, 时间, 税收状态.
* ? – 显示 /ta 指令.
* delete {玩家名} – 删除一个玩家的城镇数据.
* resident {玩家名}
* {oldname} rename {newname} – 手动给一个玩家改名. 这不需要TownyNameUpdater.jar.
* town {城镇名}
  * add {居民} .. {居民} – 邀请一个玩家到一个城镇内.
  * remove {居民} .. {居民} – 把一个玩家从城镇内移除.
  * kick {居民} – 把一个玩家踢出城镇.
  * rename {新城镇名} – 重命名一个城镇.
  * spawn – 设置一个城镇的传送点.
  * outpost # – 传送到任何城镇的前哨.
  * delete – 删除一个城镇.
  * rank {add/remove} {名称} {头衔} – 给予一个居民头衔.
* nation {国家名}
* add {城镇名} – 添加一个城镇到一个国家内.
* rename {newname} – 重命名国家.
* reset – 重置城镇 config.yml到默认状态.
* toggle
  * war – 开关战争.
  * neutral – 打开/关闭一个国家是否能宣布中立.
* npc {居民名} – 把一个玩家视为NPC,开启一个玩家的文件内的 isNPC=true, 这个玩家可以免税并且这个城镇可以免除维护费用.
* debug – 调试模式.
* devmode – 开启dev开发模式来让插件开发人员找出bug.
* withdraw – 从一个国家/城镇的银行内取钱.
* set
  * title {name} {title} – 设置一个玩家的头衔.
  * surname {玩家名} {surname} – 设置一个玩家的姓氏.
  * capital {城镇名} – 改变一个国家的国都. 这个城镇必须已加入该国家.
  * mayor
  *  {城镇名} {居民} – 设置一个居民为某城镇的城主.
  *  {城镇名} npc – 设置一个城镇的城主为NPC.
* givebonus {城镇名} {#} – 给予城镇可声明的城镇区块上限.
* reload – 重载城镇的config.yml.
* backup – 备份.
* newday – 把城镇时间跳到明天, 这并不能阻止新的一天发生.
* unclaim
* rect {范围} – 取消一块土地的声明状态.
* purge {#以天数为单位} – 删除旧的居民信息.
### /townyworld 管理员指令
缩写: /tw
* – 显示你所在世界是否启用了城镇.
* ? – 显示 /tw 指令.
* list – 列出启用城镇插件的世界.
* {world} – 显示世界设置.
* toggle
  * claimable – 开关这个世界城镇是否可以声明区块.
  * usingtowny – 开关这个世界是否启用城镇.
  * pvp – 开关这个世界的PVP.
  * forcepvp – 开关这个世界全部城镇强制开启PVP.
  * explosion – 开关这个世界的爆炸.
  * forceexplosion – 强制开启这个世界的爆炸.
  * fire – 开关这个世界的火势蔓延.
  * townmobs – 开关这个世界城镇内怪物的生成.
  * worldmobs – 强制开关世界内的怪物生成.
  * revertunclaim – 开关这个世界的回溯特性.
  * revertexpl – 开关这个世界的爆炸破坏回溯特性.
* set
  * wildname {名称} –设置荒野名.
  * wildperm {perm} .. {perm} – 不支持.
  * wildignore {id} .. {id} – 不支持.
  * wildregen {Creeper,EnderCrystal,EnderDragon,Fireball,SmallFireball,LargeFireball,TNTPrimed,ExplosiveMinecart} –设置在荒野内的哪种爆炸破坏会回溯.
* usedefault – 不支持.
* regen – 重置区块.
* undo – 撤销 /tw 重置区块.
### 城镇聊天指令
* ??? - 城镇聊天频道, 之后不需要再次输入来进入频道.
* /nationchat, /nc - 国家聊天频道, 之后不需要再次输入来进入频道.
* /global, /g - 全局聊天频道,之后不需要再次输入来进入频道.
* /a – 管理员频道.
* /m – 主持人频道.
* /channel leave|join {频道} – 离开或加入一个聊天频道.
* /ch list –列出多少玩家在你所在频道有.
* /leave {频道} – 离开一个聊天频道.
* /join {频道} – 加入一个聊天频道.
* /chmute {频道} {玩家} – 在一个频道内禁言某玩家.
* /mutelist {频道} – 显示被禁言的玩家.
* /chunmute {频道} {玩家} – 取消禁言.====