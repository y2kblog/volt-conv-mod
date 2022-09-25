# Grove・Qwiic対応 電圧変換モジュール（3.3V⇔5V）

<img src="/img/product-image-1000px.jpg" width="250px">  

I<sup>2</sup>CやUART等の信号電圧と電源電圧を変換するモジュールです。Grove互換コネクタとQwiic互換コネクタを搭載しています。  
本モジュールを使用することで3.3V系のシステムと5V系のシステムを接続できるようになります。  
以下の4パターンの電圧変換に対応しています。  

<table>
<caption>対応電圧一覧</caption>
<thead>
<tr>
    <th rowspan="2"></th>
    <th colspan="2">マスター側</th>
    <th colspan="2">スレーブ側</th>
    <th rowspan="2">例</th>
</tr>
<tr>
    <th>電源</th>
    <th>信号</th>
    <th>電源</th>
    <th>信号</th>
</tr>
</thead>
<tbody>
<tr>
    <td>①</td>
    <td>5V</td>
    <td>5V</td>
    <td>3.3V</td>
    <td>3.3V</td>
    <td>Arduino Uno → Qwiicモジュール</td>
</tr>
<tr>
    <td>②</td>
    <td>5V</td>
    <td>3.3V</td>
    <td>3.3V</td>
    <td>3.3V</td>
    <td>M5Stack Core2 → Qwiicモジュール</td>
</tr>
<tr>
    <td>③</td>
    <td>3.3V</td>
    <td>3.3V</td>
    <td>5V</td>
    <td>3.3V</td>
    <td>Raspberry Pi → M5Stackユニット</td>
</tr>
<tr>
    <td>④</td>
    <td>3.3V</td>
    <td>3.3V</td>
    <td>5V</td>
    <td>5V</td>
    <td>Raspberry Pi → Groveモジュール(5V)</td>
</tr>
</tbody>
</table>


<!-- ## 販売  
[スイッチサイエンス委託販売ページ](https://www.switch-science.com/products/xxxx/)  
※大量注文や在庫に関する問い合わせは[こちら](mailto:info.y2kb@gmail.com)までご連絡ください。   -->


## 各部の名称

<img src="/img/overview.jpg" width="400px">  


## 接続方法

<!-- 以下に示すように、 -->
マスター側とスレーブ側の電源電圧と信号電圧のパターン毎にジャンパーピンをセットしマスター・スレーブデバイスを接続してください。

- **① 電源:5V, 信号:5V→電源:3.3V, 信号:3.3V**  
  - 電圧変換方向選択ジャンパ（J4・J5）: `5V->3V3`  
  - 5Vシステム側信号電圧選択ジャンパ（J9）: `5V`  
  <img src="/img/conn_pow5Vto3v3_sig5v.jpg" width="400px">  

- **② 電源:5V, 信号:3.3V→電源:3.3V, 信号:3.3V**
  - 電圧変換方向選択ジャンパ（J4・J5）: `5V->3V3`  
  - 5Vシステム側信号電圧選択ジャンパ（J9）: `3V3`  
  <img src="/img/conn_pow5Vto3v3_sig3v3.jpg" width="400px">  

- **③ 電源:3.3V, 信号:3.3V→電源:5V, 信号:3.3V**
  - 電圧変換方向選択ジャンパ（J4・J5）: `3V3->5V`  
  - 5Vシステム側信号電圧選択ジャンパ（J9）: `3V3`  
  <img src="/img/conn_pow3v3to5v_sig3v3.jpg" width="400px">  

- **④ 電源:3.3V, 信号:3.3V→電源:5V, 信号:5V**
  - 電圧変換方向選択ジャンパ（J4・J5）: `3V3->5V`  
  - 5Vシステム側信号電圧選択ジャンパ（J9）: `5V`  
  <img src="/img/conn_pow3v3to5v_sig5v.jpg" width="400px">  


## 仕様

- 最大データレート
  - オープンドレイン（I<sup>2</sup>C等）：2 Mbps
  - プッシュプル（UART等）：24 Mbps
- 最大出力電流
  - 5V → 3.3V：1.0 A
  - 3.3V → 5V：250 mA
- 外形寸法：W32 x D40 x H11.5 mm


## 資料

### 回路図

<img src="/img/schematic_latest.png" width="500px">  

PDFファイル：<a href="https://github.com/y2kblog/volt-conv-mod/raw/master/resources/schematic_latest.pdf" >schematic.pdf</a>  

### 外形寸法

<img src="/img/dimension.png" width="350px">  

DXFファイル：<a href="https://github.com/y2kblog/volt-conv-mod/raw/master/resources/volt_conv_mod_dxf_latest.zip" download="">volt_conv_mod_dxf.zip</a>  

### 3D CADデータ

STEPファイル：<a href="https://github.com/y2kblog/volt-conv-mod/raw/master/resources/volt_conv_mod_step_latest.zip" download="">volt_conv_mod_step.zip</a>  

