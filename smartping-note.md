# smartping 功能梳理笔记 

开发分支 feature-alarm

/g/config.go 实现功能：寻找并读取配置文件


/funcs/ping.go/StartSysPing 执行ping功能，并将ping信息存储(StoragePing)

/funcs/ping.go/StartGoPing 同上
`StartSysPing 和 StartGoPing 有何区别`

PingSt 存储 ping 信息的结构体

```
type PingSt struct {
	SendPk   string
	RevcPk   string
	LossPk   string
	MinDelay string
	AvgDelay string
	MaxDelay string
}

```
阅读进度：smartping.go 第48行尚未阅读