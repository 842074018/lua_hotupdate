接口包含
- Init(RootPath, UpdateListFile [, FailNotify])
- Update()

Init负责初始化，RootPath是你的lua文件目录。UpdateListFile是一个lua路径，要求这个lua文件返回一个table，这个table包含想要热更新的文件的文件名。FailNotify是热更新出错时的函数，需要该函数接受一个字符串参数，该字符串包含了出错的原因。

Update每运行一次就对hotupdatelist里面的文件进行热更新。

限Windows平台使用，不对被更新的文件做任何假设
详细配置请看[lua closure热更新配置](http://asqbtcupid.github.io/hotupdte-implement/)




![例子动图](https://raw.githubusercontent.com/asqbtcupid/asqbtcupid.github.com/master/images/hotupdateexample.gif)