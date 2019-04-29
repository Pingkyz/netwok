# Delay 

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.15752-9/58462383_836557413384171_5973379569690869760_n.png?_nc_cat=111&_nc_eui2=AeE1Mpvw60HPm_7B8ywBxwjzH6vArM9dzGVKvx_IWTqNJV0HxKSoy0FUczqJvNJL87N0_PGPgwX2vainhWh0D6Vc3vIqN4bSX_igLY9_D32W1A&_nc_oc=AQmw4X3ZgFJxZ1gNP5a7uWqqrRTxicD0-eF15qDwbMoFQ6yrUDP-GOpjwuczU88ep7U&_nc_ht=scontent.fbkk5-3.fna&oh=804bd02c08cf7f281d8e747f5bbb2c76&oe=5D75F2B6)

## **propagation**
* คือการที่ข้อมูลเลือกเส้นทางที่เร็วที่สุด เช่น การเดินของรถโดยต้องการเดินทางจากจุด A ไปจุด B
 มีสองเส้นทางเส้นแรกความยาว12 เมตร เส้นที่2 ความยาว 8 เมตรเมื่อเส้นที่ 2คือเส้นที่สั้นที่สุดรถ
ก็จะไปทางนั้น

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.15752-9/58729736_2047874208851121_6213288119198810112_n.png?_nc_cat=111&_nc_eui2=AeGEvm9PceTpB6F5lqL7Hjl6tPLi4oVdL-dctTvNSzWQUZpsLvT25Eo4FGS4tGBNLJ-jeIcOz1vOExKSS2GHvlgA6LwsixS8Sj_-xweeS63A7Q&_nc_oc=AQmfh8sfcdmFyTH8FiyXYYmi-bogvRYuRUaVutS-csB_hJvVunR6bt29nmOUMaXGbHA&_nc_ht=scontent.fbkk5-3.fna&oh=80e5549f76cb5af6eed374e056795887&oe=5D3FCF5D)


## **Processing in Node**
* คำว่าโหนด (Node)ที่จะพูดถึงเป็น switch หรือ router ก็ได้ ซึ่งเป็นตัวกลางระห่าง
ผู้ส่งและผู้รับ เมื่อข้อมูลเดินทางมา node มันจะทำการตรวจความถูกต้องข้อมูลทุกครั้งก่อนที่จะ
เดินทางต่อไป

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.15752-9/58462383_836557413384171_5973379569690869760_n.png?_nc_cat=111&_nc_eui2=AeE1Mpvw60HPm_7B8ywBxwjzH6vArM9dzGVKvx_IWTqNJV0HxKSoy0FUczqJvNJL87N0_PGPgwX2vainhWh0D6Vc3vIqN4bSX_igLY9_D32W1A&_nc_oc=AQmw4X3ZgFJxZ1gNP5a7uWqqrRTxicD0-eF15qDwbMoFQ6yrUDP-GOpjwuczU88ep7U&_nc_ht=scontent.fbkk5-3.fna&oh=804bd02c08cf7f281d8e747f5bbb2c76&oe=5D75F2B6)


## **Transmission**
* ปริมาณการรับ และการส่งข้อมูล โดย switch หรือ router พวกนี้สามารถส่งข้อมูลได้ทุกขนาดตามที่เราส่งไปให้มัน อุปกรณ์แต่ละตัวมีสิ่งที่เรียกว่า Bandwidth อยู่ซึ่งหน่วยของมัน คิดเป็น “bps” หรือ bit per sec. “จำนวน bit ที่ส่งผ่านไปได้ในหนึ่งวินาที” นั่นเอง

## **Queueing**
*  เป็นช่วงเวลาที่ข้อมูลถูกหน่วงก่อนที่จะส่งต่อไป สาเหตุของความหน่วงคือข้อมูลที่มีมากจนnode
ทำงานไม่ทัน nodeตัวหนึ่งจะมีการเชื่อมต่อระหว่างผู้ส่งแลัผู้รับหลายตัว แล้วตัวที่เชื่อมต่อมันจะ
ส่งข้อมูลออกมาพร้อมๆกัน เมื่อข้อมูลเยอะมากมันจะจัดการโดยให้ switch หรือ router
 จะพักข้อมูลที่เข้ามาพักเอาไว้หรือที่เรียกว่า buffer คือพักก่อนและค่อยๆจัดการข้อมูล
# **unit (หน่วย)**
## **time (เวลา)**
* หน่วยวัดเวลามาตราฐานส่วนใหญ่เราก็ใช้ “second หรือ วินาที” นั่นแหละ แต่เนื่องจากคอมพิวเตอร์และอุปกรณ์อิเล็กโทรนิคมันทำงานเร็วมาก! ถ้านับเป็นวิก็คงต้องพูดกันเป็น 0.00005 วิอะไรแบบนั้น

ในเมื่อมันน้อยมากๆ เลยจะใช้ ms (millisec. มิลลิวินาที)

![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.15752-9/58740008_2330868737202860_7015377505154498560_n.png?_nc_cat=101&_nc_oc=AQliHbCdj9hJUHJwi0pZySGBQr3xCEV3zUiUcYl4gL7LBK_OZQJw3QY-6D8wFA8Z8Ys&_nc_ht=scontent.fbkk5-6.fna&oh=612e68652b3911ba8a18f07abc6d54d8&oe=5D2A14CF)
# **Data (ข้อมูล)**
* ข้อมูลที่จะส่งจะนับกันเป็น
bits การส่งข้อมูลจริงๆ จะส่งแบบ 011100101001 คอมพิวเตอร์รู้จักแค่เลขฐานสอง ซึ่งมันก็สะดวกดีนะเวลาส่งแต่ถ้าให้คนมาคิดก็ต้องปวดหัวกันนิดหน่อย คือส่งทีละ bit
ดังนั้นถ้าเขาให้ byte มาก็ต้องเอาไป คูณ8 ให้เป็น bit ก่อนถึงจะตอบได้

# **transmission(การส่ง)**
* ให้ข้อมูลผ่านในหนึ่งหน่วยเวลา คือ
วิ.นึงเนี่ยให้ข้อมูลผ่านไปได้กี่ตัว โดยจะนับเป็น

![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.15752-9/58614632_1476392842497107_2404326295778361344_n.png?_nc_cat=101&_nc_oc=AQnlttXE_ZP6GwHkWbDG_HSNoBLjPeXhQ9m3dxj6p9wVGEWXMxQuAR4xNFPWivPISD4&_nc_ht=scontent.fbkk5-6.fna&oh=a4570e02cc8f654d0cb7d2fe0d8b432f&oe=5D6853A4)

ถ้าเป็นระบบคอม 1 วิ.จะส่งได้เป็นล้านต้วเลยมีการเพิ่ม เมก้า(Mega)ไปเป็น Mbps
# **Total-delay Time**
คือการคำนวนหน่วยเวลาที่กล่าวมา บวกกันทั้งหมดจะได้ว่า
![
](https://scontent.fbkk5-1.fna.fbcdn.net/v/t1.15752-9/57362465_347886232395647_6198192919766106112_n.png?_nc_cat=109&_nc_oc=AQk3gEbHTWZk3GUHA4cNJEwNjW85w2gj99IPE_ETHVE2bznyAB_OZUIgba6nQ3fPG4c&_nc_ht=scontent.fbkk5-1.fna&oh=f477fc3f59452dcacfdf1ca6805f57ce&oe=5D72228B)
