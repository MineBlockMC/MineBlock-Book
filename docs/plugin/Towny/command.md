# 命令

### `/towny` 城镇指令

* `（无子命令）` - 展示基本的城镇指令.
* `?` - 展示更多城镇指令.
* `farmblocks` - 显示在农场领地内可使用的方块.
* `itemuse` - 显示 item\_use\_ids 列表里的物品.
* `map` - 展示城镇地图.
  * `hud` - 启用玩家计分板的地图.
* `plotclearblocks` - 显示使用 `/plot clear` 删除的方块
* `prices` - 展示城镇税收和维护费用.
* `switches` - 展示 switch\_ids 列表内的方块.
* `time` –展示到下一天的时间 (征收税收/维持费.)
* `top` 排行
  * `residents {all/town/nation}` - 列出所有/城镇/国家的居民列表.
  * `land {all/resident/town}` - 展出拥有土地最多的人.
* `spy` - 管理员指令,窥视所有聊天频道的信息
* `tree` - 显示大量内容.只能在后台使用
* `universe` - 显示所有城镇的数据, 居民/城镇/国家/世界 已声明的城镇区块计数.
* `v` - 显示插件版本.
* `wildsblocks` - 显示在荒野领地能使用的方块，和在荒野能进行耕种的方块

### `/plot` 领地指令

* `（无子命令）` - 展示 /plot 指令.
* `claim` - 居民用来购买出售的土地的指令.
  * `auto` - 居民用来自动购买附近出售中的土地的指令.
* `unclaim` - 居民放弃自己的土地的指令.
  * `circle/rect` - 自动放弃区域内的自己的土地.(圆形/矩形 下同)
  * `{# (以当前位置半径)}` - 放弃土地的半径.
* `{forsale/fs}` - 出售一块土地.
  * `circle/rect` - 设置选区形状.
    * `{# (以当前位置半径)}` - 出售土地的半径.
  * `$` - 土地价格.
    * `circle/rect` - 设置选区形状.
      * `{# (以当前位置半径)}` - 出售土地的半径.
* `{notforsale/nfs}` - 设置土地无法出售.
  * `circle/rect` - 设置选区形状.
    * `{# (以当前位置半径)}` - 设置无法出售的土地的半径.
* `evict` - 移除一个领地拥有者的领地，通常由镇长或是助理执行.
* `trust`
  * `add {name}` - 把玩家添加为领地的信任者.
  * `remove {name}` - 移除玩家的领地信任者身份.
* `perm` - 展示玩家所在区块的权限.
  * `gui` - 开启一个菜单来配置领地的权限覆盖.
  * `add {name}` - 为一个玩家添加领地的权限覆盖.
  * `remove {name}` - 移除一个玩家的领地权限覆盖.
* `perm hud` - 开关显示更多土地权限信息的hud计分版.
* `set`
  * `reset` - 把其他类型的土地重置为普通的土地.
  * `shop` - 设置土地为商店.
  * `embassy` - 设置领地为大使馆.
  * `arena` - 设置领地为竞技场.
  * `wilds` - 设置领地为荒野.
  * `inn` - 设置领地为旅店.
  * `jail` - 设置领地为监狱.
  * `farm` - 设置领地为农场.
  * `bank` - 设置领地为银行.
  * `outpost` - 设置领地为前哨, 与 /t claim outpost 花费相同.
  * `name` - 允许城镇或地主重命名地名, 覆盖默认的\~Unowned message.个人土地会显示地主名和地名.
  * `perm` - 编辑土地权限
    * `{on/off}` - 启用/关闭权限限制.
    * `{resident/ally/outsider} {on/off}` -开关 居民/盟友/外来者 的权限 [See here for details.](https://github.com/TownyAdvanced/Towny/wiki/How-Towny-Works#towny-plot-perms)
    * `{build/destroy/switch/itemuse} {on/off}` -开关 建筑/破坏/开关/物品使用 权限
    * `{resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}` -开关 居民/盟友/外来者 的 建筑/破坏/开关/物品使用 权限
    * `reset` - 重置领地权限为 /town 或 /resident 上的默认权限 (取决于是地主还是他人使用该指令)
* `toggle`
  * `fire` - 开关你所站土地的火势蔓延.
  * `pvp` - 开关你所站土地的PVP.
  * `explosion` - 开关你所站土地的爆炸.
  * `mob` - 开关你所站土地的怪物生成.
* `clear` - 回溯土地归于原生, 只会回溯配置内指定类型的方块.
* `group`
  * `add|new|create {groupname}` - 在玩家所站的地方创建一个领地组，同时把领地添加到现有组中。
  * `remove` - 从领地组中删除该领地.
  * `delete` - 完全删除一个领地组.
  * `rename {newname}` - 重命名一个领地组.
  * `set {plottype}` - 将一个领地组设置为特定的领地类型. 不能用于监狱类型的领地组.
  * `set perm ...` - 用来为你所站的领地组设置权限行.有关其余命令的详细信息，请参见上一节的/plot set perm.
  * `toggle ...` - 用来切换领地的设置. 有关其余命令的详细信息，请参见上一节的/plot set toggle.
  * `forsale|fs {price}` - 以给出的价格将领地组设置为在售.
  * `notforsale|nfs` - 取消领地组的在售状态.
  * `trust`
    * `add {name}` - 将一个玩家添加到领地组的信任名单中.
    * `remove {name}` - 将一个玩家移除出领地组的信任名单.
  * `perm` - 展示玩家所在区块的权限.
    * `gui` - 开启一个菜单来配置领地的权限覆盖.
    * `add {name}` - 为一个玩家添加领地的权限覆盖.
    * `remove {name}` - 移除一个玩家的领地权限覆盖.
* `jailcell`
  * `add` - 在玩家所站的地方设立一间牢房，如果领地种类是监狱的话.
  * `remove` - 移除玩家所站立的地方的牢房，如果领地种类是监狱的话.

### `/resident` 个人指令

缩写: `/p`, `/res` \*\`\`\` - 展示resident相关指令.

* `?` - 展示 /res 可用的命令.
* `{resident}` - 显示另一居民的信息.
* `friend`
  * `add {resident} .. {resident}` - 居民将在线玩家添加到好友列表中.
  * `add+ {resident} .. {resident}` - 居民将离线玩家添加到好友列表中.
  * `remove {resident} .. {resident}` - 居民将在线玩家移除出好友列表.
  * `remove+ {resident} .. {resident}` - 居民将离线玩家移除出好友列表.
  * `clearlist` - Removes all friends from a resident's friend list.
  * `list` - Returns a list of your friends.
* `list` - Lists residents in towny's data folder who are online.
* `jail paybail` - Allows a player to pay to get out of jail. Funds go to the town which owns the Jail.
* `spawn` - If deny\_bed\_use: true and player has a current bed spawn, command will teleport player to their bed.
* `toggle`
  * `map` - Turns on map which refreshes when moving across plot borders.
  * `townclaim` - Turns on mode where /town claim is automatically used when moving across plot borders.
  * `plotborder` - Turns on smokey plot-border view. Border shows when players cross to different townblocks.
  * `constantplotborder` - Turns on smokey plot-border view. Border doesn't disappear.
  * `spy` - Admins can turn on chat-channel spying.
  * `ignoreplots` - Turns on/off plot notifications in town.
  * `reset` - This turns off all modes that are active.
* `set`
  * `perm`
    * `{on/off}` - Edits the perm line on the resident screen. See here for details.
    * `{friend/ally/outsider} {on/off}`
    * `{build/destroy/switch/itemuse} {on/off}`
    * `{friend/ally/outsider} {build/destroy/switch/itemuse} {on/off}`
    * `reset` - This takes the perm line seen in the /resident screen and applies it to all plots personally owned by the player typing it.
* `tax {resname}` - Shows taxes a player pays.

### `/town` 城镇指令

缩写: `/t`

* `（无子命令）` - 展示玩家所在的城镇信息.
* `?` - 展示可用的/town指令.
* `{城镇名}` - 显示某个城镇的信息.
* `here` - 显示你所站在的那个城镇的信息.
* `leave` - 离开城镇.
* `list {page #}` - 列出城镇列表.
  * `by name {page #}` - order alpabetically.
  * `by resident {page #}` - order by town with most residents.
  * `by balance {page #}` - order by town with the highest nation bank balance.
  * `by townblocks {page #}` - order towns by how many townblocks they have claimed.
  * `by online {page #}` - order by how many players are online at that moment.
  * `by open {page #}` - lists open towns first, in order of most residents to least residents.
  * `by public {page #}` - lists public towns first, in order of most residents to least residents.
  * `by ruined {page #}` - lists ruined towns first, in order of most residents to least residents.
  * `by bankrupt {page #}` - lists bankrupt towns first, in order of most residents to least residents.
  * `by founded {page #}` - order by founded date, oldest first.
* `online` - 显示你所在城镇的在线玩家.
* `plots {城镇名}` - 展示城镇内的土地及其种类和税收.
* `new`
  * `{城镇名}` - 创建新城镇.
  * `{城镇名} {城主}` - 创建城镇(管理员指令).
* `add {居民} .. {居民}` - 邀请玩家到你的城镇内(城主指令).
* `kick {居民} .. {居民}` - 把一个玩家踢出你的城镇(城主指令).
* `invite` - Show a list of players who've been sent invites to your town.
  * `sent` - Show a list of players who've been sent invites to your town.
  * `received` - Show a list of invites your town has received from nations.
  * `accept {nationname}` - Accept an invite to join a nation.
  * `deny {nationname}` - Deny an invite to join a nation.
  * `{playername}` - Send an invite to a player to join your town.
* `spawn` - 传送到城镇出生点.
* `spawn {城镇名}` - 传送你到其他城镇的出生点.
* `claim` - 声明你所在的区块为城镇所有(管理员/助手指令).
  * `outpost` - 为你的城镇建立前哨.
  * `{# (以当前位置为半径)}` - 声明附近的区块为你的城镇所管辖.
  * `auto` - 尽可能多地自动声明你附件的区块为你的城镇所管辖.
* `unclaim` - 放弃管辖当前区块.
  * `all` - 放弃管辖所有城镇区块(城主指令).
  * `{# (以当前位置为半径)}` - 放弃附近的区块为你的城镇所管辖.
  * `outpost` - 用于放弃前哨 on MySQL Towny servers pre-0.92.0.0
* `withdraw {$}` - 从城镇银行内取钱.
* `deposit {$}` - 捐钱给城镇.
* `baltop {townname}` - Opens a book displaying the richest players in a town.
* `bankhistory {#}` - Opens a book GUI with # number of transactions listed, showing the town bank history.
* `buy`
  * `bonus {amount}` - 购买可用城镇区块上限.
* `allylist {townname}` - Displays a list of allies for the Town.
* `enemylist {townname}` - Displays a list of enemies for the Town.
* `delete {town name}` - 删除城镇及其数据(管理员/城主指令)(解散城镇使其分崩离析).
* `merge {town name}` - {town name} is the town which will be merged into the town owned by the mayor using the command.
* `outlawlist {城镇名}` - 列出城镇放逐者列表.（92版本才有）
* `outlaw {add/remove} {name}` –从城镇放逐者列表中添加或移除玩家（92版本才有）
* `outpost`
  * `{# (#相当于相应的前哨编号)}` - 传送到一个前哨.
  * `{list}` - 列出你的城镇前哨.
* `plotgrouplist {townname} {page #}` - Lists a town's plotgroups with forsale and price indicated.
* `purge {days}` - Kicks residents from the town who have been inactive for the given number of days, exempts npcs and mayors.
* `ranklist` - 展示居民头衔.
* `rank {add|remove} {玩家名} {头衔名}` - 给予或移除一个居民的头衔.
* `reclaim` - allows a resident to reclaim their ruined town.
* `reslist {城镇名}` - 查看一个城镇内的所有居民.
* `say {msg}` - 向城镇成员广播信息.
* `set`
  * `board {信息}` - 设置公告栏信息(居民在每次登录时会看到的信息).
    * `{message}` - Sets message seen by residents upon logging in.
    * `none` - Sets an empty board which will not be seen on login or in the /town status screen.
  * `mayor {居民}` - 将你的城主之位传给下一代(城主指令).
  * `homeblock` - 设置城镇中心区块(传送点).
  * `spawn` - 设置城镇传送点, 必须在城镇中心区块内.
  * `spawncost` - Set the cost of spawning to a public town. Doesn't affect town residents, nation members and nation-allies.
  * `mapcolor {color}` - Sets a town's mapcolor seen in the dynmap.
  * `name {名称}` - 改变你的城镇名.
  * `outpost` - 设置一个城镇区块为前哨.
  * `jail` - 重置监狱的传送点到你所在的位置.
  * `perm` - 城镇权限设置
    * `{on/off}` - 开关
    * `{resident/ally/outsider} {on/off}` - 开关 居民/盟友/外来者 权限
    * `{build/destroy/switch/itemuse} {on/off}` - 开启或关闭 建筑/破坏/开关/物品使用 权限
    * `{resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}` - 开关 居民/盟友/外来者的 建筑/破坏/开关/物品使用 权限
    * `reset` - 这个指令将会重置城镇内所有的领地权限为默认领地设置.
  * `tag` {最多4个标签}\`\`\` - 设置城镇标签(可改变聊天的格式).
    * `clear` - 清除城镇标签.
  * `taxes {$}` - 设置固定的每日税收. 也可以设置为税收率.
  * `taxpercentcap {$}` - The maximum amount that can be taken when taxpercent is enabled.
  * `plottax {$}` - 设置土地税, 按照居民拥有的土地数来收税.
  * `plotprice {$}` - 设置城镇的默认土地价格.
  * `shopprice {$}` - 设置默认的商店领地价格.
  * `shoptax {$}` - 设置商店领地税, 按照拥有的商店领地来收税.
  * `embassyprice {$}` - 设置默认大使馆领地价格.
  * `embassytax {$}` - 设置大使馆领地税, 按照拥有的大使馆领地来收税.
  * `title {name} {titlegoeshere}` - Mayor command to add a Title to a member of the town.
  * `surname {name} {surnamegoeshere}` - Mayor command to add a Suffix to a member of the town.
  * `primaryjail` - Sets your town's primary jail.
* `toggle`
  * `explosion` - 开关城镇内的爆炸.
  * `fire` - 开关城镇内的火势蔓延.
  * `mobs` - 开关城镇内的敌对怪物生成.
  * `public` - 对外人是否开启城镇传送点.
  * `pvp` - 开关城镇内的PVP.
  * `taxpercent` - 开关按税率收税.
  * `nationzone` - Turn on/off the town's NationZone.
  * `open` - 开放/关闭公开城镇.
* `join {城镇名}` - 加入公开的城镇.
* `jail`
  * `list` - Shows jail number, name, coord, cellcount and which jail is the primary jail.
  * `{name}` - Jails the given player for 1 hour, must be a resident of your own town.
  * `{name} {hours}` - Jails the given player for the given hours.
  * `{name} {hours} {jail}` - Jails the given player for the given hours, in the given jail plot (which is a number.)
  * `{name} {hours} {jail} {cell}` - Jails the given player for the given hours, in the given jail plot and jail cell (which are both numbers.)
* `unjail {name}` - Unjails someone in your town's jail.
* `trust`
  * `add {name}` - Adds a player as Trusted to the entire town.
  * `remove {name}` - Removes a player from being Trusted by the entire town.

### `/nation` 国家指令

缩写: `/n`, `/nat`

* `（无子命令）` - 显示玩家所在国家的情况.
* `?` - 显示 /nation 指令.
* `list {页码}` - 列出所有国家.
  * `by name {page #}` - order alpabetically.
  * `by resident {page #}` - order by nation with most residents across all towns.
  * `by balance {page #}` - order by nation with the highest nation bank balance.
  * `by towns {page #}` - order by nation with the most towns.
  * `by townblocks {page #}` - order nations by how many townblocks their towns have collectively claimed.
  * `by online {page #}` - order by how many players are online at that moment.
  * `by open {page #}` - ordered by open first, number of residents second.
  * `by public {page #}` - order by public first, number of residents second.
  * `by founded {page #}` - order by founded date, oldest first.
* `online` - 显示在线的国人.
* `{国家名}` - 显示某个国家的信息.
* `leave` - 从祖国的怀抱中挣脱(城主指令).
* `withdraw {$}` - 从国库中取钱(国王指令).
* `deposit {$}` - 捐钱给国家.
* `baltop {nationname}` - Opens a book displaying the richest players in a nation.
* `bankhistory {#}` - Opens a book GUI with # number of transactions listed, showing the nation bank history.
* `deposit {$} {townname}` - King command to add money to the bank of a town who is in the nation.
* `new`
  * `{国家名}` - 建国.
  * `{国家名} {国都}` - 创建新的国家并设置某个城镇为国都(管理员指令).
* `rank` - 设置国家内的助手/自定义头衔.
* `add {城镇名}` .. {城镇名}\`\`\` - 邀请一个城镇加入你的国家.
* `kick {城镇名}` .. {城镇名}\`\`\` - 把一个城镇踢出你的国家.
* `delete {国家名}` - 灭国 (国王指令).
* `invite` - Show a list of invites sent.
  * `help` - Show a list of invites sent.
  * `sent` - Show a list of invites sent.
  * `{town}` - Invites a town to a nation.
* `ally`
  * `add {国家名} .. {国家名}` - 把一个国家视为盟国.
  * `remove {国家名} .. {国家名}` - 不再把一个国家视为盟国.
  * `accept {nationname}` - Accepts an invitation to ally from another nation.
  * `deny {nationname}` - Denies an invitation to ally from another nation.
  * `sent` - Show a list of nation alliance invites sent.
  * `received` - Show a list of nation alliance invites received.
* `enemy`
  * `add {国家名} .. {国家名}` - 把一个国家视为敌国.
  * `remove {国家名} .. {国家名}` - 不再把一个国家视为敌国.
* `rank {add|remove} {玩家名} {头衔名}` - 给予一个玩家国家头衔.
* `say {msg}` - 广播信息给在线的国民.
* `set`
  * `king {居民}` - 把一个玩家加冕为王.
  * `captial {城镇名}` - 设置国都.
  * `board`
    * `{message}` - Sets message seen by residents upon logging in.
    * `none` - Sets an empty board which will not be seen on login or in the /nation status screen.
  * `taxes {$}` - 设置国税.
  * `name {国名}` - 设置国家名.
  * `spawn` - Sets the nation spawn point.
  * `spawncost` - Sets the cost of public spawns to that nation's spawn point. No effect on members of the nation or nation-allies
  * `title {名称} {头衔内容}` - 给国家添加头衔(国王指令).
  * `surname {名称} {surnamegoeshere}` - 给国民冠以姓氏(国王指令).
  * `tag` {最多4个标签}\`\`\` - 设置国家标签.
    * `clear` - 清除国家标签.
  * `mapcolor {color}` - Sets the colour seen on the dynmap-towny webpage.
* `toggle`
  * `neutral` - 是否设置你的国家在战争期间每日付费来保持中立.
  * `open` - Sets the nation to be open, so that any town can join without an invite.
* `join {nation}`
  * Used by a town mayor to join an open nation.
* `merge {nationname}`
  * Requests the given nation to merge into your nation.
  * Can only be used by the nation king, and requires the king of the other nation to be online to accept the merger.
  * The soon-to-be-ex-king will receive a confirmation message asking if they will accept the dissolution of their nation.
  * If accepted the towns of the nation transfer to the remaining nation. The nation's bank money is also transferred.
* `ranklist {nationname}` - Displays residents and their ranks, optional nationname to view another nation's rank list.
* `townlist (nation)`
  * (nation) is optional, to show townlist of a nation you aren't a part of.
  * lists all towns in a nation.
* `allylist (nation)`
  * (nation) is optional, to show allylist of a nation you aren't a part of.
  * lists all allies of a nation.
* `enemylist (nation)`
  * (nation) is optional, to show enemylist of a nation you aren't a part of.
  * lists all enemies of a nation.

### `/townyadmin` 管理员指令

缩写: `/ta`

* `（无子命令）` - 显示内存, 线程, 战争状态, 生命恢复设置, 时间, 税收状态.
* `?` - 显示 /ta 指令.
* `tpplot {world} {x} {z}` - Teleports an admin to the Towny chunk coordinates seen in the /towny map command. Be careful with large numbers, you could be teleported farther than you think and end up generating chunks.
* `plot`
  * `claim {playername}` - Admin command to claim a plot for another player. Area must be a part of a town.
  * `meta` - used to view a plot's metadata.
  * `set [key] [value]` - Sets a metadata.
  * `[add|remove] [key]` - Adds or removes a metadata.
  * `claimedat` - Shows when the plot was claimed.
* `resident`
  * `{residentname} delete` - Admin command to delete a resident.
  * `{oldname} rename {newname}` - Admin command to manually rename a resident to a new name. Not need if TownyNameUpdater.jar is present.
  * `{residentname} friend [add|remove|clear|list]` - Allows admins to manipulate a resident's friends list.
  * `{residentname} unjail` - Admin command to unjail any resident.
* `town new {townname} {mayor}` - Admin command to create a town for the mayor where the command sender is standing, does not charge money.
* `nation new {nationname} {capital}` - Admin command to create a nation for the capital town, does not charge money.
* **Dep** `resident {玩家名}`
* **Dep** `{oldname} rename {newname}` - 手动给一个玩家改名. 这不需要TownyNameUpdater.jar.
* `town {城镇名}`
  * `add {居民} .. {居民}` - 邀请一个玩家到一个城镇内.
  * `invite {resident}` - Admin command to send a town invite to a player.
  * `remove {居民} .. {居民}` - 把一个玩家从城镇内移除.
  * `kick {居民}` - 把一个玩家踢出城镇.
  * `rename {新城镇名}` - 重命名一个城镇.
  * `spawn` - 设置一个城镇的传送点.
  * `outpost #` - 传送到任何城镇的前哨.
  * `delete` - 删除一个城镇.
  * `rank {add/remove} {名称} {头衔}` - 给予一个居民头衔.
  * `toggle [any /t toggle command]...` - Use a town's toggles for them.
  * `forcepvp` - Set the town's AdminEnabledPVP setting to true or false.
  * `set [any /t set command]...` - Use a town's set command for them.
  * `meta` - used to view a town's metadata.
  * `set [key] [value]` - Sets a metadata.
  * `[add|remove] [key]` - Adds or removes a metadata.
  * `outlaw [add|remove] [name]` - Admin command to add/remove outlaws from a town.
  * `leavenation` - Admin command to make a town leave their nation.
  * `deposit [amount]` - Deposit money into a town's bank.
  * `withdraw [amount]` - Withdraw money from a town's bank.
  * `bankhistory {#}` - Opens a book GUI with # number of transactions listed, showing the town bank history.
  * `unruin` - Un-ruins a ruined town.
* `nation {国家名}`
  * `add {城镇名}` - 添加一个城镇到一个国家内.
  * `rename {newname}` - 重命名国家.
* `reset` - 重置城镇 config.yml到默认状态.
* `toggle`
  * `neutral` - 打开/关闭一个国家是否能宣布中立.
  * `npc {居民名}` - 把一个玩家视为NPC,开启一个玩家的文件内的 isNPC=true, 这个玩家可以免税并且这个城镇可以免除维护费用.
  * `debug` - 调试模式.
  * `devmode` - 开启dev开发模式来让插件开发人员找出bug.
  * `withdraw` - 从一个国家/城镇的银行内取钱.
  * `wildernessuse (on|off)` - Turns on/off the build/destroy/switch/itemuse properties of all worlds.
  * `regenerations (on|off)` - Toggles explosion regen and unclaimed revert in the wilderness of each world off or on.
* `set`
  * `plot {town}` - Sets a plot to a town.
    * When in a town only a single plot can be transfered at one time. Does not require a town to have available townblocks to claim.
    * When in the wilderness two types of sub commands can be used to do area claims:
    * Does require a town to have available townblocks to claim.
    * Does obey proximity rules for claims between towns/homeblocks.
    * /ta set plot {town} {rect|circle} {radius}
    * /ta set plot {town} {rect|circle} auto
  * `title {name} {title}` - 设置一个玩家的头衔.
  * `surname {玩家名} {surname}` - 设置一个玩家的姓氏.
  * `capital {城镇名}` - 改变一个国家的国都. 这个城镇必须已加入该国家.
  * `mayor`
    * `{城镇名} {居民}` - 设置一个居民为某城镇的城主.
    * `{城镇名} npc` - 设置一个城镇的城主为NPC.
  * `nationzoneoverride [town] [size]` - Sets a town's NationZone size.
* `givebonus {城镇名} {#}` - 给予城镇可声明的城镇区块上限.
* `depositall {amount}` - Deposits given amount to all town and nation banks.
* `reload` - 重载城镇的config.yml.
  * `all` - Reloads everything.
  * `database` - Reloads the database.
  * `perms` - Reload the townyperms.yml.
  * `config` - Reloads the config.yml.
  * `lang` - Reloads the language file.
* `backup` - 备份.
* `checkperm {player} {node}` - Quick test of whether a player has a permission node.
* `newday` - 把城镇时间跳到明天, 这并不能阻止新的一天发生.
* `unclaim`
  * `rect {范围}` - 取消一块土地的声明状态.
* `purge {#以天数为单位}` - 删除旧的居民信息.
  * Optional townless flag will limit purge to only residents who are not part of a town.
* `purge {# as in days} {townname}` - Deletes old residents.
  * Optional townname flag will limit purge to only residents who are a part of that town.
* `mysqldump`
  * When your config has save & load set to mysql you can use this command to dump the mysql database to flatfile.
* `database`
  * `[save|load]` - Saves or loads the database.
  * `remove titles` - Removes all titles and surnames from all residents.
* `townyperms`
  * `grouplist` - Lists all the groups in the townyperms.yml
  * `group [groupname]` : lists the nodes held by a group.
  * `group [groupname] addperm|removeperm [node]` : adds or removes a node to/from a group.
  * `townrank addrank|removerank [rank]` : adds or removes a town rank.
  * `nationrank addrank|removerank [rank]` : adds or removes a nation rank.

### `/townyworld` 管理员指令

缩写: `/tw`

* `（无子命令）` - 显示你所在世界是否启用了城镇.
* `?` - 显示 /tw 指令.
* `list` - 列出启用城镇插件的世界.
* `{world}` - 显示世界设置.
* `toggle`
  * `claimable` - 开关这个世界城镇是否可以声明区块.
  * `usingtowny` - 开关这个世界是否启用城镇.
  * `pvp` - 开关这个世界的PVP.
  * `forcepvp` - 开关这个世界全部城镇强制开启PVP.
  * `friendlyfire` - Turn on/off whether town/nation/allied members can hurt each other.
  * `explosion` - 开关这个世界的爆炸.
  * `forceexplosion` - 强制开启这个世界的爆炸.
  * `fire` - 开关这个世界的火势蔓延.
  * `townmobs` - 开关这个世界城镇内怪物的生成.
  * `worldmobs` - 强制开关世界内的怪物生成.
  * `wildernessmobs` - Turn on/off the mobs listed in the wilderness mobs in the wilderness.
  * `revertunclaim` - 开关这个世界的回溯特性.
  * `revertentityexpl` - Turn on/off the reverting of explosions by entities in the wilderness feature for that world.
  * `revertblockexpl` - Turn on/off the reverting of explosions by blocks in the wilderness feature for that world.
  * `warallowed` - Turn on/off whether war plugins should operate in this world.
  * `plotcleardelete` - Turn on/off whether the /plot clear command can be used.
  * `unclaimblockdelete {on|off}` - Turns on/off the delete-blocks-on-unclaim feature in the world.
* `set`
  * `wildname {名称}` - 设置荒野名.
  * `wildperm {perm} .. {perm}` - 不支持.
  * `wildignore {id} .. {id}` - 不支持.
  * `wildregen {Creeper,EnderCrystal,EnderDragon,Fireball,SmallFireball,LargeFireball,TNTPrimed,ExplosiveMinecart}` - 设置在荒野内的哪种爆炸破坏会回溯.
  * `usedefault` - 不支持.
* `regen` - 重置区块.
* `undo` - 撤销 /tw 重置区块.

### `/invite`

* `（无子命令）` - 显示子命令.
* `?|help` - 显示子命令.
* `list` - 显示你收到的邀请列表
* `accept {town}` - 接受加入一个城镇的邀请.
* `deny {town}` - 拒绝加入一个城镇的邀请.

### 城镇聊天指令

* `/townychat reload` - 重载 chatconfig.yml 和 channels.yml
* `/townchat`, `/tc` - 城镇聊天频道, 之后不需要再次输入来进入频道.
* `/nationchat`, `/nc` - 国家聊天频道, 之后不需要再次输入来进入频道.
* `/global`, `/g` - 全局聊天频道,之后不需要再次输入来进入频道.
* `/res set mode reset` - 重置聊天模式为默认.
* `/a` - 管理员频道.
* `/m` - 助理者频道.
* `/channel leave|join {频道}` - 离开或加入一个聊天频道.
* `/ch list` –列出多少玩家在你所在频道有.
* `/leave {频道}` - 离开一个聊天频道.
* `/join {频道}` - 加入一个聊天频道.
* `/chmute {频道} {玩家}` - 在一个频道内禁言某玩家.
* `/mutelist {频道}` - 显示被禁言的玩家.
* `/chunmute {频道} {玩家}` - 取消禁言.