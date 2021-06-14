#### 物聯網裝置(Netgear WNAP320 AP)模擬
在這次的實作中，我們選擇使用Docker搭配QEMU模擬無線AP裝置
#### 為何選擇使用Docker部署
- Docker可以讓我們建立起的模擬裝置更加容易執行，分享，以及修改
- 在Docker中可以安全地模擬惡意軟體以及感染裝置
#### QEMU
- Open source的裝置模擬器
- User space emulation可以模擬不同架構的裝置，對於大部分採用MIPS/ARM架構的IOT裝置模擬十分有幫助
- 有提供許多的架構支援\
![QEMU](qemu.png)


#### 執行問題
- IOT裝置模擬耗時且複雜(CPU架構不同)
- 裝置韌體須透過特殊方法才能將架構解析

#### 實驗步驟
- 
