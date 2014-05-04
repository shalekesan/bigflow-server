bigflow-server
==============

Bigflow是一个用于IT运营自动化的流程设计、调度工具. 


产品描述
-------------------

Bigflow流程调度管理产品由后台流程调度服务程序和前端流程设计程序组成，采用基于插件的体系架构。
默认支持的任务类型包括远程脚本、存储过程，可以根据需要以插件方式扩展更多任务类型。
支持定时触发、定制日历触发和文件到达触发三种流程触发方式。可用于各种IT系统任务调度管理。

更多信息请参考 http://www.doggadata.com/

环境要求
------------
    * Java >= 1.7 (OpenJDK and Sun have been tested)

使用说明
---------------

win安装服务端
	
	  * 安装mysql
    	  * 解压 bigflow-server-$VERSION.rar
    	  * 把bigflow-server下db目录下的表导入mysql
    	  * 修改conf/bigflow_server.properties文件中mysql和jms配置
    	  * cd bigflow-server-$VERSION/bat
    	  * runConsole.bat运行服务端
    	  * installService.bat安装服务
    	  * startService.bat启动服务
    	  * stopService.bat停止服务
    	  * uninstallService.bat卸载服务

注意: 启动后可在win的系统托盘上起、停等管理服务.

win安装客户端
	
	  * 下载bigflow-client-$VERSION.rar并解压
	  * 双击setup.exe安装
	  * 进入到安装目录，修改conf/bigflow_server.properties文件中mysql和jms配置
	  * 启动即可
