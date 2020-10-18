# erp_pro

> 基于SpringBoot 2.X框架，为中小企业打造开源好用的ERP软件。主要模块有零售管理、采购管理、销售管理、仓库管理、财务管理、报表查询、系统管理等。支持预付款、收入支出、仓库调拨、组装拆卸、订单，生产等特色功能。拥有库存状况、出入库统计等报表。对权限进行精确划分，同时支持多系统集成方案，可与OA，CRM，知识库等多个系统进行集成使用。同时对角色和权限进行了细致全面控制，精确到每个按钮和菜单。集成apollo配置中心。`项目长期更新，觉得不错的点下star吧`

- erp+生产演示视频：https://www.bilibili.com/video/BV1yA411e7mm/
- 项目交流群：(群一：[696070023](http://shang.qq.com/wpa/qunwpa?idkey=e9aace2bf3e05f37ed5f0377c3827c6683d970ac0bcc61b601f70dc861053229))(群二：[836039567](https://shang.qq.com/wpa/qunwpa?idkey=7bb6f29b27f772aadca9c7c4e384f7833c64e9c3c947b5e946c7b303d1fe174a))(群三：[887391486](https://shang.qq.com/wpa/qunwpa?idkey=a65f2e0292eb1048bb13abb7adca302bd83e3465974861ec1f04c2f7fffc4d99))`商业需求直接进微信群，申请QQ群的直接拒绝`
- 需要进微信群的，进微信群需要支付五元费用(加我拉你进群，wzq_598748873)，为了防止发广告的等，喜欢爱答不理的就别进，进了也会被踢。望谅解。
- `不想支付的进QQ群，别尼玛加了我微信说这说那的`
- 工作清单以及价格表：https://docs.qq.com/doc/DQlRxcVRMWWVjbU1i?_from=1&disableReturnList=1
- [OA地址](https://gitee.com/doc_wei01/skyeye)
- 不会搭建环境的，可以出钱让作者帮忙搭建，一次100，先付。
- 环境搭建资料以及项目介绍操作文档（50一份）获取：进群后找群主

#### 功能介绍

功能|描述|功能|描述
---|---|---|---
用户管理|用户是系统操作者，该功能主要完成系统用户配置|部门管理|配置系统组织机构（公司、部门、小组），树结构展现支持数据权限
岗位管理|配置系统用户所属担任职务|菜单管理|配置系统菜单，操作权限，按钮权限标识等
角色管理|角色菜单权限分配、设置角色按机构进行数据范围权限划分|基础设置|包含背景图片设置、锁屏图片设置等
计量单位|产品规格单位管理|结算账户|自定义账户的结算方式以及结算明细的查看
收支(科目)项目|自定义除了采购/销售等产生的费用外，其他产生费用的项目|基本资料|包含会员管理、供应商管理,商业版客户已抽离为CRM
库存管理(商业版)|对比开源版新增库存管理，可以查看每个商品不同规格的库存数|工序管理(商业版)|管理每个商品自产的流程工序
BOM表(商业版)|为自产商品打造结构清单，清晰了解成本价等|生产计划(商业版)|销售计划单直接生成生产计划（也可以手动下达生产计划），可根据BOM表自动生成半成品生产计划
采购管理|包含采购单、转入库单、采购入库、采购退货等功能，整改完成|销售管理|包含销售单、转出库单、销售出库、销售退货等功能，整改完成
其他入库管理|整改完成|库存盘点|对现有仓库的库存进行盘点
待审核入库单(商业版)|仓库管理员可以对自己仓库的入库单进行审核入库|待审核出库单(商业版)|仓库管理员可以对自己仓库的出库单进行审核出库
零售管理|包含零售出库、零售退货等功能，整改完成|拆分单|整改完成
调拨单|整改完成|仓库管理|管理用户所拥有的仓库,整改完成
商品管理|管理用户所拥有的产品信息,整改完成|组装单|整改完成
待审核其他单据(商业版)|包含组装单，拆分单，调拨单的审核|加工单信息(商业版)|根据生产计划单下达部门加工单，完成成品的加工
领料单(商业版)|部门领料单管理|补料单(商业版)|部门补料单管理
退料单(商业版)|部门退料单管理|部门存量管理(商业版)|部门拥有的物料存量管理
加工单(商业版)|成品加工流程完成|其他单据管理|包含其他入库、其他出库、调拨、组装单、拆分单等功能
报表管理|包含入库/出库明细、入库/出库汇总、库存状况、客户/供应商/会员对账等报表|财务管理|收入单、支出单、收付款单、转账单等
工艺路线管理(商业版)|工艺路线设计|车间管理(商业版)|生产车间管理
加工机器管理(商业版)|工厂加工机器|手机端(商业版)|erp+生产模块手机端功能

#### 技术选型

##### 后端技术:

技术|名称|版本
---|---|---
[SpringBoot](http://spring.io/projects/spring-boot)|核心框架|2.0.3
[MyBatis](http://www.mybatis.org/mybatis-3/zh/index.html)|ORM框架
[Druid](https://github.com/alibaba/druid)|数据库连接池|
[Maven](http://maven.apache.org/)|项目构建管理|
[redis](https://redis.io/)|key-value存储系统|3.2集群（不要问我单机的能不能行）
[webSocket](http://www.runoob.com/html/html5-websocket.html)|浏览器与服务器全双工(full-duplex)通信|
[quartz](http://www.quartz-scheduler.org/)|定时任务|2.2.2
[ActiveMQ](http://activemq.apache.org/replicated-leveldb-store.html)|消息队列|
[Java]()|Java|1.8
[MySQL]()|数据库|5.5.28

##### 前端技术：

技术|名称
---|---
[jQuery](http://jquery.com/)|函式库
[zTree](http://www.treejs.cn/v3/)|树插件
[layui](https://www.layui.com/)|模块化前端UI
[winui](https://gitee.com/doc_wei01/skyeye)|win10风格UI(自己做的前端架构)
[handlebars](http://www.ghostchina.com/introducing-the-handlebars-js-templating-engine/)|js模板引擎
[webSocket](http://www.runoob.com/html/html5-websocket.html)|浏览器与服务器全双工(full-duplex)通信

#### 代码描述
##### 前后台接口映射

```
<url id="前端请求id" path="后台接口" val="备注" allUse="是否需要登录">
	<property id="前端请求key" name="后台接收key" ref="限制条件（参考项目内文档）" var="key含义"/>
</url>
```

##### 后台代码编写规范

###### 控制层

```
@RequestMapping("后台接口")
public void 方法名(InputObject inputObject, OutputObject outputObject) throws Exception{
	服务层接口对象.方法名(inputObject, outputObject);
}
```

###### 服务层

```
@Override
public void 方法名(InputObject inputObject, OutputObject outputObject) throws Exception {
	Map<String, Object> map = inputObject.getParams();//接收参数
	Map<String, Object> user = inputObject.getLogParams();//获取当前登录用户信息
	/**
	 * 业务逻辑
	 */
	outputObject.setBean(bean);//返回单个实体Bean
	outputObject.setBeans(beans);//返回集合
	outputObject.settotal(total);//返回数量
	outputObject.setreturnMessage("信息");//返回前端的错误信息
	outputObject.setreturnMessage("信息", 错误码);//返回前端的错误信息，同时抛出异常（不常用）
}
```

#### 效果图

|效果图|效果图|
| ------------- | ------------- |
|![](https://images.gitee.com/uploads/images/2019/1011/084458_e0c2e256_1541735.png "")|![](https://s2.ax1x.com/2019/10/11/uHSaY8.png "")|
|![](https://images.gitee.com/uploads/images/2019/1011/084630_9326c93d_1541735.png "")|![](https://s2.ax1x.com/2019/10/11/uHpkh8.png "")|
|![](https://images.gitee.com/uploads/images/2019/1011/084706_8c921d85_1541735.png "")|![](https://s2.ax1x.com/2019/10/11/uHpeXj.png "")|
|![](https://images.gitee.com/uploads/images/2019/1015/091741_4030a2f0_1541735.png "")|![](https://s2.ax1x.com/2019/10/15/K9meR1.png "")|
|![输入图片说明](https://images.gitee.com/uploads/images/2019/1022/165203_457e90a8_1541735.png "在这里输入图片标题")|![输入图片说明](https://images.gitee.com/uploads/images/2019/1022/165318_c88d74e3_1541735.png "在这里输入图片标题")|
|![输入图片说明](https://images.gitee.com/uploads/images/2019/1022/165355_a7090ee3_1541735.png "在这里输入图片标题")|![输入图片说明](https://images.gitee.com/uploads/images/2019/1022/165505_0f5c5162_1541735.png "在这里输入图片标题")|
|![输入图片说明](https://images.gitee.com/uploads/images/2019/1022/165537_fbb78be8_1541735.png "在这里输入图片标题")|![输入图片说明](https://images.gitee.com/uploads/images/2019/1023/152325_95480f53_1541735.png "在这里输入图片标题")|

### 捐助
如果您觉得我们的开源软件对你有所帮助，请扫下方二维码打赏我们一杯咖啡。
| 支付宝 | 微信 |
| ------ | ---- |
| ![      ](https://images.gitee.com/uploads/images/2019/1016/094014_96f92c56_1541735.png "微信截图_20191016093832.png") | ![     ](https://images.gitee.com/uploads/images/2019/1016/094025_65ba24f0_1541735.png "微信截图_20191016093850.png")|
