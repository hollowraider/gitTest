# Hyperledger Fabric第一次启动

Hyperledger Fabric的示例项目test-network，下载地址：



1. 环境装备：windows上推荐WSL，下载一个ubuntu环境
2. 需要安装必要软件：docker、docker compose、git、go、jq
3. 代理配置，在国内代理必须配
	- docker代理
	- go代理
4. install-fabric.sh脚本，脚本包含了docker镜像、示例项目和二进制文件，必须下载
	- github替换代理网址，国内github下载巨慢，可以替换github代理加速[https://ghp.ci/](https://ghp.ci/)
5. 按照教程启动







chaincode安装失败

更新go版本，wsl中的默认go版本是1.13。最好和教程中一致，当时是要求1.23.3，从官网手动下载。



tidy安装失败

![image-20241202020911593](Hyperledger Fabric第一次启动.assets/image-20241202020911593.png)

很奇怪，之后进入了/asset-transfer-basic/chaincode-go，手动使用`go mod tidy`显示安装成功，再次运行chaincode命令安装成功

之后安装成功

![image-20241202021207845](Hyperledger Fabric第一次启动.assets/image-20241202021207845.png)



