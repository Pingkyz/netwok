# Delay 

## Delay ประกอบด้วย
### **propagation**
* คือการที่ข้อมูลเลือกเส้นทางที่เร็วที่สุด เช่น การเดินของรถโดยต้องการเดินทางจากจุด A ไปจุด B
 มีสองเส้นทางเส้นแรกความยาว12 เมตร เส้นที่2 ความยาว 8 เมตรเมื่อเส้นที่ 2คือเส้นที่สั้นที่สุดรถ
ก็จะไปทางนั้น

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.15752-9/58729736_2047874208851121_6213288119198810112_n.png?_nc_cat=111&_nc_eui2=AeGEvm9PceTpB6F5lqL7Hjl6tPLi4oVdL-dctTvNSzWQUZpsLvT25Eo4FGS4tGBNLJ-jeIcOz1vOExKSS2GHvlgA6LwsixS8Sj_-xweeS63A7Q&_nc_oc=AQmfh8sfcdmFyTH8FiyXYYmi-bogvRYuRUaVutS-csB_hJvVunR6bt29nmOUMaXGbHA&_nc_ht=scontent.fbkk5-3.fna&oh=80e5549f76cb5af6eed374e056795887&oe=5D3FCF5D)


### **Processing in Node**
* คำว่าโหนด (Node)ที่จะพูดถึงเป็น switch หรือ router ก็ได้ ซึ่งเป็นตัวกลางระห่าง
ผู้ส่งและผู้รับ เมื่อข้อมูลเดินทางมา node มันจะทำการตรวจความถูกต้องข้อมูลทุกครั้งก่อนที่จะ
เดินทางต่อไป

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.15752-9/58462383_836557413384171_5973379569690869760_n.png?_nc_cat=111&_nc_eui2=AeE1Mpvw60HPm_7B8ywBxwjzH6vArM9dzGVKvx_IWTqNJV0HxKSoy0FUczqJvNJL87N0_PGPgwX2vainhWh0D6Vc3vIqN4bSX_igLY9_D32W1A&_nc_oc=AQmw4X3ZgFJxZ1gNP5a7uWqqrRTxicD0-eF15qDwbMoFQ6yrUDP-GOpjwuczU88ep7U&_nc_ht=scontent.fbkk5-3.fna&oh=804bd02c08cf7f281d8e747f5bbb2c76&oe=5D75F2B6)


### **Transmission**
* ปริมาณการรับ และการส่งข้อมูล 

### **Queueing**
*  เป็นช่วงเวลาที่ข้อมูลถูกหน่วงก่อนที่จะส่งต่อไป สาเหตุของความหน่วงคือข้อมูลที่มีมากจนnode
ทำงานไม่ทัน nodeตัวหนึ่งจะมีการเชื่อมต่อระหว่างผู้ส่งแลัผู้รับหลายตัว แล้วตัวที่เชื่อมต่อมันจะ
ส่งข้อมูลออกมาพร้อมๆกัน เมื่อข้อมูลเยอะมากมันจะจัดการโดยให้ switch หรือ router
 จะพักข้อมูลที่เข้ามาพักเอาไว้หรือที่เรียกว่า buffer คือพักก่อนและค่อยๆจัดการข้อมูล