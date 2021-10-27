# Network Devices
![網路設備Network Devices](./pic/networkdevices.png)

## L1 Devices
### [中繼器 Repeater](https://zh.wikipedia.org/wiki/%E4%B8%AD%E7%BB%A7%E5%99%A8)
  - 增強放大輸入訊號
  - 不考慮輸入訊號種類
### [集線器 Hub](https://zh.wikipedia.org/wiki/%E9%9B%86%E7%B7%9A%E5%99%A8)
  - 可視作有多個埠的中繼器
  - 連接多條雙絞線或光纖
  - 連結的裝置工作在同一網段
  - 現已被 [交換器(Switch)](#交換器-switch) 取代
#### Cons:
  - 訊號之間碰撞機會大
  - 訊號可被竊聽
## L2 Devices
### [交換器 Switch](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E4%BA%A4%E6%8F%9B%E5%99%A8)
  - 使用[MAC位址](https://zh.wikipedia.org/wiki/MAC%E5%9C%B0%E5%9D%80)([Media Access Control Address](https://en.wikipedia.org/wiki/MAC_address))轉發資料
  - 只將資料轉發到需要接收的裝置
## L3 Devices
### [路由器 Router](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8)
  - 連接兩個"以上"個別網路的裝置
  - 安裝相關的軟體，可使普通電腦變成路由器
  - 路由:決定封包從來源端到目的端所經過的路徑(host到host之間的傳輸路徑)
  - 轉送:輸入端的封包移送至適當的輸出端(裝置內部進行)
#### 無線網路路由器
  - 用來連繫有線和無線網路
  - 易受環境影響連接速度
#### [原則型路由](https://zh.wikipedia.org/wiki/%E5%8E%9F%E5%89%87%E5%9E%8B%E8%B7%AF%E7%94%B1)
  - 也稱"策略路由"
  - 額外定義路由-轉發的規則，包含策略與操作，稱為路由圖
  - 作用於介面上，檢查其接收到的所有封包是否符合路由圖中的策略，符合的以路由圖對應的操作來處裡，不符合以常規路由處理
