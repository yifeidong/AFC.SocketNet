# AFC.SocketNet
一、项目情况
  我们的工作主要是研发各城市的轨道交通自动售检票通迅系统AFC（参与的项目有天津地铁6号线、武汉地铁21号线、长春北湖线、深圳龙华有轨电车等城市的售检票系统）。因不同的城市会有不同的通迅标准协议，所以每个不同城市的AFC在准备前期，都必须花费大量的时间去实现通迅模块(以TCP的长连接为主)。而且这些通迅模块会涉及到售检票系统交易数据、设备状态、软件更新等重要操作，是一个重中之重的模块。所以有必要针对此特殊情况，以不变应万变，在短时间内快速简单地完成通迅模块的开发工作，并能最大限度保证通迅服务的稳定性和满足高客流的高并发性能。
 
 二、项目介绍
  基于上述情况，特意把一直在变在通迅协议抽离出来，独立在可配置的配置文件中；把不变的通迅处理机制封装起来。可根据不同城市的通迅协议标准进行配置，就能自动快速生成可复用的TCP通迅框架。
 
