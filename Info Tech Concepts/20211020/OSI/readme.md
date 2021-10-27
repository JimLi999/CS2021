# About OSI
![網路設備Network Devices](https://github.com/JimLi999/CS2021/blob/main/Info%20Tech%20Concepts/20211020/pic/networkdevices.png)
## L1 [實體層](https://zh.wikipedia.org/wiki/%E7%89%A9%E7%90%86%E5%B1%82) [Physical Layer](https://en.wikipedia.org/wiki/Physical_layer)
  - 為傳輸資料，需要"物理"鏈路與裝置的建立、維持、拆除，並具有機械的、電子的、功能的、規範的特性
### 功能
  - 為資料端裝置提供傳送資料通路
  - 傳輸資料
### 常見裝置
  - [集線器](https://github.com/JimLi999/CS2021/tree/main/Info%20Tech%20Concepts/20211020/NetworkDevices#%E9%9B%86%E7%B7%9A%E5%99%A8-hub)
  - [中繼器](https://github.com/JimLi999/CS2021/tree/main/Info%20Tech%20Concepts/20211020/NetworkDevices#%E4%B8%AD%E7%B9%BC%E5%99%A8-repeater)

## L2 [資料連結層](https://zh.wikipedia.org/wiki/%E6%95%B0%E6%8D%AE%E9%93%BE%E8%B7%AF%E5%B1%82) [Data Link Layer](https://en.wikipedia.org/wiki/Data_link_layer)
  - transfers data between nodes on a network segment across the physical layer 在網段上的節點與實體層之間傳輸數據
  - 兩個網路實體之間提供資料鏈路連接的建立、維持和釋放管理
### 功能
  - 提供導線的一端到另一端的資料傳輸
  - 會在 frame 尾端置放檢查碼（parity，sum，CRC）以檢查實質內容，將實體層提供的可能出錯的物理連接改造成邏輯上無差錯的資料鏈路
  - 資料封裝:包含了位址段和資料段等。
      - 位址段:含有點對點傳送節點和接收節點的位址（如MAC）
      - 控制段:用來表示數格連接影格的類型
      - 資料段:包含實際要傳輸的資料
### 協定
  - [VLAN](https://zh.wikipedia.org/wiki/%E8%99%9A%E6%8B%9F%E5%B1%80%E5%9F%9F%E7%BD%91) ([IEEE 802.1Q](https://zh.wikipedia.org/wiki/IEEE_802.1Q))
  - [乙太網](https://zh.wikipedia.org/wiki/%E4%BB%A5%E5%A4%AA%E7%BD%91) ([IEEE 802.3](https://zh.wikipedia.org/wiki/IEEE_802.3))
  - [Wi-Fi](https://zh.wikipedia.org/wiki/Wi-Fi) ([IEEE 802.11](https://zh.wikipedia.org/wiki/IEEE_802.11))
### 常見裝置
  - [交換器](https://github.com/JimLi999/CS2021/tree/main/Info%20Tech%20Concepts/20211020/NetworkDevices#%E4%BA%A4%E6%8F%9B%E5%99%A8-switch)
  - [網卡](https://zh.wikipedia.org/wiki/%E7%BD%91%E5%8D%A1)
  - [橋接器](https://zh.wikipedia.org/wiki/%E6%A9%8B%E6%8E%A5%E5%99%A8)

## L3 [網路層](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E5%B1%82) [Network layer](https://en.wikipedia.org/wiki/Network_layer)
  - 提供路由和尋址的功能
### 功能
  - 定址
    - 使用IP位址來唯一標識網際網路上的裝置
    - 依靠IP位址進行相互通訊
    - 編址方案
      - [IPv4](https://zh.wikipedia.org/wiki/IPv4)
      - [IPv6](https://zh.wikipedia.org/wiki/IPv6)
  - 路由
    - "不同的網路"之間相互通訊
### 協定
  - [IPv4](https://zh.wikipedia.org/wiki/IPv4)
  - [IPv6](https://zh.wikipedia.org/wiki/IPv6)
  - [IPsec](https://zh.wikipedia.org/wiki/IPsec)
### 常見裝置
  - [路由器](https://github.com/JimLi999/CS2021/tree/main/Info%20Tech%20Concepts/20211020/NetworkDevices#%E8%B7%AF%E7%94%B1%E5%99%A8-router)
  - [三層交換器](https://en.wikipedia.org/wiki/Multilayer_switch#Layer-3_switching)
## L4 [傳輸層](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E5%B1%82) [Transport layer](https://en.wikipedia.org/wiki/Transport_layer)
  - 應用行程提供端到端的通訊服務
  - 提供面向連接的資料流支援、可靠性、流量控制、多路復用等服務
### 服務
  - 通過傳輸層協定的編程介面傳遞給應用行程
    - [連接導向式通訊](https://zh.wikipedia.org/wiki/%E9%80%A3%E6%8E%A5%E5%B0%8E%E5%90%91%E5%BC%8F%E9%80%9A%E8%A8%8A)
    - 相同次序交付
    - [可靠性](https://zh.wikipedia.org/wiki/%E5%8F%AF%E9%9D%A0%E6%80%A7_(%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C))
    - [流量控制](https://zh.wikipedia.org/wiki/%E6%B5%81%E9%87%8F%E6%8E%A7%E5%88%B6_(%E6%95%B0%E6%8D%AE))
    - [擁塞避免](https://zh.wikipedia.org/wiki/%E6%8B%A5%E5%A1%9E%E6%8E%A7%E5%88%B6)
    - [多路復用](https://zh.wikipedia.org/wiki/%E5%A4%9A%E8%B7%AF%E5%A4%8D%E7%94%A8)
### 協定
  - [TCP](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE)
  - [UDP](https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE)
  - [SPX](https://zh.wikipedia.org/wiki/SPX)
