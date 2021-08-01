# **ADNS-9800**
ADNS-9800 sensor breakout board for use with trackball/mouse. Compatible with 3.3V and 5V Vcc (via jumper settings).
![](/img/sensor1.jpg)

## [Project page on EasyEDA](https://easyeda.com/pigboard/adns9800board)

## **BOM**
|Name               |Value   |Footprint         |Qty   |
|:---:              |:---:   |:---:             |:---: |
|C1                 |10nF    |0805              |1     |
|C2                 |1uF     |SMD_L3.2-W1.6-R-RD|1     |
|C3                 |470pF   |0805              |1     |
|C4,C5,C6,C7        |100nF   |0805              |4     |
|C8                 |3.3uF   |SMD_L3.2-W1.6-R-RD|1     |
|C9                 |4.7uF   |SMD_L3.2-W1.6-R-RD|1     |
|C10, C11           |10uF    |SMD_L3.2-W1.6-R-RD|2     |
|DMOSI,DNCS,DSCLK   |3.3V    |SOD-323           |3     |
|RMOSI,RNCS,RSCLK   |330 Ohm |0805              |3     |
|T1                 |        |SOT-416           |1     |
|ADNS-9800 + lens   |        |                  |1     |

Optional (for easier prototyping)
|Name               |Qty   | Notes |
|:---:              |:---: |:---   |
|H1                 |1     |8 pin (2x4) 2.54 pitch male through hole pin header|
|JP1                |1     |2 pin 2mm pitch male through hole pin header|
|JP2                |1     |3 pin 2mm pitch male through hole pin header|
|JPC                |2     |2 pin 2mm pitch jumper cap|


Remarks:
*   Diodes are 3.3V Zener diodes
*   T1 is NTA4151PT1G transistor
*   Jumpers and 8 pin male header are only usefull if you're planning to change operational voltage frequently and plug sensor to different devices, otherwise just soldering the jumpers for correct operational volatage and data wire is sufficient
*   Jumper cap is usefull for selecting operational voltage
*   Sensor together with the lens can be obtained from [Aliexpress](https://www.aliexpress.com/item/32954048411.html?spm=a2g0o.productlist.0.0.71b7788dw8yPsj&algo_pvid=7c0317d9-86de-4067-a4e8-24debb8c6201&algo_exp_id=7c0317d9-86de-4067-a4e8-24debb8c6201-0)
*   Check below for an easy way to order most of the parts


## **Ordering (low volume)**
Head over to [JLCPCB](https://jlcpcb.com/) and click 'Quote now'. Here choose 'Add gerber file' and upload  **ADNS9800.zip** file from **'gerber'** folder. Use the default settings.

![](/img/lowvoldef.png)

Altenratively you can order directly from the project page at [EasyEDA](https://easyeda.com/pigboard/adns9800board). Scroll down to 'ADNS9800 Board Drop In Replacement' and choose 'Open in editor'. There you can click 'PCB Fabrication file' icon. 

![](/img/easyeda1.png)

Either 'Check DRC' or just generate gerber and as a last step click 'Order at JLCPCB' on the bottom right. 

##  **Ordering (higher volume)**
You can increase number of PCB's without spending a lot of money. In order to do so you will have to use panelization. With the project opened in the editor choose 'Tools->Panelize...'. Use settings below. Don't lower column/row count as this the minimum that can be manufactured. But you can increase it freely.

![](/img/panelize1.png)

### **Ordering parts**
You can order most of the parts with few clicks. Open the schematic from the project page on EasyEDA. From there click 'BOM...' icon and then 'Order parts/Check stock'.

![](/img/easyeda2.png)

This will open LCSC page where you have to change one column and mark it as 'LCSC Part number'. Click 'Next' and remove parts that are not available etc.

![](/img/lcsc1.png)





