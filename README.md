# hospital_parent
医院预约挂号管理系统


项目模块创建：
hospital_parent：根目录，管理所有子模块
  common:公共模块父节点
      common-util:工具类模块，所有模块依赖它
      rabbit-util:rabbitmq业务封装
      service-util:service服务工具包，包含service服务的公共配置类，所有service模块依赖它
  
  service-gateway:服务网关
  model:实体类模块
  service：api接口服务
      service-hosp:医院api接口服务
      service-cmn:公共api接口服务
      service-user:用户api接口服务
      service-order:订单api接口服务
      service-sms:短信api接口服务
      service-task:定时任务服务
      service-statistics：统计api接口服务
  
  service-client：feign服务调用父节点
      service-cmn-client:公共api接口
      service-hosp-client：医院api接口
      service-order-client：订单api接口
