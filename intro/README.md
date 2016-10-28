## Crayfish

Crayfish 是一个前端配置管理系统。与一般的配置管理系统不同的是 Crayfish 是将配置发布到 CDN，前端程序直接从 CDN 加载，对后端服务器不会造成任何压力。

## 应用场景

### 1. 文案管理

很多前端的文案都会频繁修改，最典型的就是用户交易平台的用户协议和帮助中心。以前都是产品经理提出文案修改需求，然后再让开发人员排期修改，最后还要发布到代码。

后来我们将文案部分抽取到 Crayfish 中，并且把编辑权限直接交给产品经理。这样不仅节省了开发的时间，还可以让产品经理更加及时地修改文案。

### 2. 开关管理

以前涉及到需要动态控制的地方我们都会让后端开发接口，把后端作为配置管理器。

后来遇到了限时抢购这个业务，由于并发非常高，这么搞会把后端打挂。

于是我们把开关放到了 Crayfish 上，由于是纯 CDN 的，没有服务器性能瓶颈，轻松扛下秒杀配置开关的任务。

### 3. 更多玩法等你来折腾！

Crayfish 的作用远不止上面列举的，我们正在把它推向 App、推向后端……

## 特点

* 配置在 CDN 上，没有服务器性能瓶颈
* 健壮的权限机制，可以从角色和项目两个维度管理权限
* 配置是有数据类型的，让前端程序可以更准确地使用