ORDER_SERVICE
=============

订单系统的Service服务端
小结：
1.数据库设计将业务拆分成最小实体单元后通过对其封闭形成产品
2.Service和Controller采用RPC远程调用，实现分布部署
3.Service通过业务逻辑实现多表信息拼结形成前台页面展示的View类
4.Service不做任何数据检验，只实现业务逻辑的调用
5.Controller负责View的展示和接收数据的准确性
6.为了前台数据传入的一至性，我采用所有Parameter都使用String类型，转换放在Service去实现
