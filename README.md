# tomcat-deploy
完成多节点，多业务，部署脚本（不用key免认证方式）
发布需求
依赖最小的脚本bash或者python 最基础的包
功能需求
一个配置文件，含业务名称定义、业务对应iplist、uzn 业务服务器密码（目前都一样）、tomcat目录、备份目录、备份重命名规则、发布目录
一个执行脚本
1.完成读取配置
2.从app13节点 发布目录自动copy 发布包到对应节点 
3.appp13copy 配置文件到对应发布节点：
3.1提供重启每个节点或全部tomcat功能
4.发布前自动备份、清理过期备份，最多保存3份发布包。