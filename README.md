# Covid-19 Situation Impact on Commodity prices
![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/bbb89762-1753-4abc-a80e-514389032ba9)


## Background (Hypothesis)
    
จากสถานะการณ์Covid-19 ที่เป็นโรคภัยระบาดครั้งใหญ่ของโลกซึ่งเป็นโรคติดต่อร้ายแรงที่เกิดขึ้นมาใหม่ในเมืองอู่ฮั่นในประเทศจีนเดือนธันวาคมปี2019 
โดยไวรัสชนิดนี้เป็นชนิดใหม่ที่ไม่เคยพบเจอที่ไหนมาก่อน เป็นโรคภัยพิบัติที่ทำให้เกิดความวิตกกังวลอย่างมากต่อชีวิตของคนทั่วโลกยาวมาถึงปัจจุบัน 
จากกราฟด้านบนเราแบ่งTimelineของสถาณการณ์เป็น5ช่วงหลักๆ
    
- 1.ช่วงค้นพบโรคCovid-19 และ เริ่มระบาดทั่วโลก
- 2.ช่วงของปิดประเทศและการกักตัวตามนโยบายควบคุมโรคในแต่ละประเทศ
- 3.ช่วงเริ่มต้นของการผ่อนคลายและเริ่มเปิดพรหมแดนระหว่างประเทศ
- 4.ช่วงที่ประกาศCovid-19 เป็นเชื้อโรคประจำถิ่นและเปิดให้มีกิจกรรมสันทนาการ
- 5.ช่วงนี้ประเทศจีนเปิดเผยรายงานการติดเชื้อภายในประเทศ

ประกอบกับช่วงเวลาที่ผ่านมาเกิดสภาวะตลาดสินค้าโภคภัณฑ์ที่มีการปรับตัวของราคาสินค้าอย่างผันผวน เราจึงเริ่มตั้งคำถามในสิ่งที่เราสนใจ

## คำถามที่เกิดขึ้น
- 1.สถานะการณ์การระบาดของCovid-19ทั่วโลกส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ในปัจจุบันมากหรือน้อยเพียงใด ?
- 2.กลุ่มของสินค้าโภคภัณฑ์กลุ่มใดได้รับหรือเสียประโยชน์จากสถานะการณ์Covid-19 อย่างไร ?


[Grace] คาดว่าจำนวนผู้ติดเชื้อโควิดตั้งแต่เริ่มมีการประกาศภาวะฉุกเฉินในเดือนมกราคม ปี 2563 เป็นต้นมา ส่งผลต่อราคาผันผวนของสินค้าโภคภัณฑ์ในตลาดโลก เนื่องจากปัจจัยในการส่งออก-นำเข้า, กำลังการผลิต หรือ ความต้องการใช้สินค้าโภคภัณฑ์ในแต่ละประเภท เป็นต้น
ดังนั้น EDA ที่จะนำเสนอต่อไปนี้ จึงเป็นการวิเคราะห์จากราคาสินค้าโภคภัณฑ์ในแต่ละประเภทควบคู่ไปกับจำนวนผู้ติดเชื้อโควิดรายวันทั่วโลก เพื่อให้เห็นถึงความสัมพันธ์ของ 2 ข้อมูลดังกล่าว ......
  
### ศึกษาผลกระทบของสินค้าโภคภัณฑ์จากการะบาดของโควิด-19 [Grace]ประเภทของสินค้าโภคภัณฑ์... เพิ่มอีก ## อธิาบเรื่องการแบ่งช่วงสีแดงในแต่ละช่วง --> definition คืออะไร
## เราทำการแบ่งกลุ่มของสินค้าโภคภัณฑ์หลักเป็น 5 ประเภท 
- `1.สินค้าโภคภัณฑ์ประเภทพลังงาน`
  - ได้แก่ น้ำมันดิบ, ก๊าซธรรมชาติ, น้ำมันให้ความร้อน และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้เป็นสินค้าที่มีปริมาณความต้องการเป็นจำนวนมาก เพราะ เป็นปัจจัยสำคัญต่อระบบขนส่งขนาดใหญ่ทั่วโลก และยังเป็นสินค้าหลักในการผลิด 
    พลังงานและความร้อนแก่อุตสาหกรรมหนักขนาดใหญ่และครัวเรือน
    
- `2.สินค้าโภคภัณฑ์ประเภทโลหะ`
  - ได้แก่ ดีบุก, ตะกั่ว, อะลุมิเนียม, เงิน, ทองคำ, นิกเกิล, สังกะสี, พาลาเดียม และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้ใช้เป็นวัตถุดิบในหลายอุตสาหกรรมหนัก ไม่ว่าจะเป็นอุตสาหกรรมเครื่องใช้ไฟฟ้าหรืออุปกรณ์อิเล็กทรอนิกส์จนไปถึงอุตสาหกรรมเพื่อความงาม  
    และบางสินค้าอย่างเช่นทองคำ ยังอยู่ในกลุ่มของ "โลหะมีค่า" (Precious Metal) เพื่อการลงทุนในระยะยาวอีกด้วย
    
- `3.สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์`
  - ได้แก่ เนื้อหมู, เนื้อวัว, เนื้อไก่ และ อื่นๆ
  - สินค้าประเภทนี้อาจจะดูคล้ายกับสินค้าทางการเกษตรแต่สินค้าที่มาจากสัตว์เพื่อการบริโภค
   
- `4.สินค้าโภคภัณฑ์ประเภทการเกษตร`
  - ได้แก่ กาแฟ, โกโก้, ไม่แปรรูป, น้ำตาล, น้ำส้ม และอื่นๆ
  - สินค้าประเภทการเกษตรเป็น Soft commodity หรือผลิตภัณฑ์จากการเพราะปลูกจะมีอายุเก็บรักษาที่จำกัดไม่สามารถเก็บได้ไว้นานซึ่งมีความผันผวนของราคา
    ค่อนข้างสูงเนื่องจากปัจจัยเสี่ยงที่ไม่สามารถคุมได้อาทิ สภาพอากาศ, ปริมาณน้ำ เป็นต้น
     
- `5.สินค้าโภคภัณฑ์ประเภทเมล็ดพืช`
  - ได้แก่ ข้าวสาลี, ข้าวโอต, ข้าวโพด, ถั่วเหลือง, น้ำมันถั่วเหลือง และ อื่นๆ
  - สินค้าประเภทนี้เป็นสินค้าที่สามารถบริโภคได้ด้วยตรงและเป็นสินค้าที่สามารถเป็นผลิตภัณฑ์แปรรูปได้อาทิ แป้งข้าวโพด, ขนมปัง เพื่อเป็นการบริโภคทางอ้อม
    รวมไปถึงเป็นอาหารของสัตว์ที่จำถูกนำมาบริโภคในลำดับถัดๆไป

## กราฟแสดราคาสินค้าโภคภัณฑ์แต่ละประเภทเพื่อหาข้อสรุป
### 1.สินค้าโภคภัณฑ์ประเภทพลังงาน

![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

  ข้อสรุป
  - เกิดการหยุดใช้พลังงานอย่างกระทันหันเนืองจากการระงับเดินทางในประเทศและต่างประเทศรวมไปถึงการหยุดบริโภคพลังงานจากโรงงาน ในส่วนของผู้ผลิตน้ำมันสู้ 
    ตลาดไม่สามารถหยุดการผลิตได้เนื่องจากต้นทุนในการเริ่มเครื่องจักร ทำให้ราคน้ำมันดิบมีราคาติดลบ
  - หลังจากเริ่มเปิดประเทศในช่วงนี้ไตรมาส4ปี2021 ราคาน้ำมันทุกประเภทเริ่มค่อยๆฟื้นตัวตอนเริ่มเปิดประเทศ จนไปถึงช่วงที่การท่องเที่ยวเริ่มฟื้นตัวจากมาตรการผ่อน 
    คลายสถานะกาณ์ทำให้ราคาน้ำมันกลับสู่ปกติ
    
### 2. สินค้าโภคภัณฑ์ประเภทโลหะ

![metal](https://github.com/bsssgrace/5001-mini-project/assets/114140787/cf81e1c7-e15a-4ce3-a478-4cd06623f2f3)

  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์ประเภทโลหะไม่ได้มีความสัมพันธ์กับอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื่อโควิดอาจจะต้องหาปัจจัยอื่นมาอธิบายเพิ่มเติม
  - ทองคำเป็นสินค้าเพื่อการลงทุนและนิยมซื้อเก็บเพื่อรักษาความเสี่ยงทางการเงินที่ราคาปรับตัวสูงขึ้นอย่างโดดเด่นเนื่องจากสถานะการโควิด
  - การลดจำนวนผู้ติดเชื้อCovid-19 ไม่ได้ส่งผลให้ความความผันผวนของราคาโลหะลดลง 

### 3.สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์

![meat](https://github.com/bsssgrace/5001-mini-project/assets/114140787/63a1a9f9-f8eb-40a6-889a-1a1d173630ee)

  ข้อสรุป
  - จากกราฟจะสังเกตุเห็นว่าราคาเนื้อสัตว์(เนื้อหมู,เนื้อวัว)ที่พร้อมสำหรับบริโภคมีแนวโน้มราคาที่ปรับตัวสูงขึ้นอยู่ตลอดไม่ได้สัมพันธ์กับจำนวนยอดผู้ติดเชื้อโควิด ซึ่งราคาที่ 
    ปรับตัวขึ้นของสินค้าประเภทนี้น่าจะมาจากปัยจัยอื่นเช่นอัตราเงินเฟ้อ โดยทำให้เราสามารถตัดปัจจัยจากยอดผู้ติดเชื่อโควิดได้ 

### 4. สินค้าโภคภัณฑ์ประเภทการเกษตร

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/e2722d68-8b64-4170-bfe1-71289e538451)


  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์ประเภทการเกษตรไม่ได้มีความสัมพันธ์กับอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื่อโควิดอาจจะต้องหาปัจจัยอื่นมาอธิบายเพิ่มเติม

### 5. สินค้าโภคภัณฑ์ประเภทเมล็ดพืช

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/8951642b-ca9d-430d-9628-a82b070bc5b0)

  #### ข้อสรุป
  - สินค้าโภคภัณฑ์ประเภทนี้มีการปรับราคาโดยรวมสูงขึ้นไปในทางเดียวกันกับโภคภัณฑ์ประเภทเนื้อสัตว์โดยราคาปัจจุบันยังไม่สามารถกลับไปในช่วงก่อนเกิดสถานการณ์โควิดได้
  - ราคาข้าวเปลือกมีราคาที่สูงขึ้นอย่างโดดเด่นในช่วงไตรมาส1-2 ของปี 2020 อย่างโดดเด่น แต่เมื่อทำการค้นหาข้อมูลเพิ่มพบปัจจัยราคาที่สูงขึ้นเกิดการ 
    กักตุนสินค้าจากผู้ผลิตรายใหญ่อย่างเวียดนาม (ไม่ได้เ้กี่ยวข้องกับสถานะการCovid-19แต่อย่างใด)

## Overall Summary & Next Action Plan

1. สถานะการณ์การระบาดของCovid-19ทั่วโลกส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ในปัจจุบันมากหรือน้อยเพียงใด ?
    - ผลกระทบจากสถานะการณ์Covid-19 มีผลทำให้ทุกสินค้าโภคภัณฑ์ทุกประเภทมีราคาที่ต่ำลงอย่างเห็นได้ชัดในช่วงแรกของการระบาดและ                            
      ราคาสินค้าเริ่มฟื้นตัวกลับสู่ราคาเดิมระเวลาต่อมา และเริ่มปรับตัวสูงขึ้นโดยไม่เกี่ยวข้องกับการระบาดของCovid-19
    - สินค้าโภคภัณฑ์ที่ได้รับผลกระทบอย่างชัดเจนในช่วงแรกของการระบาดคือราคาน้ำมัน(ติดลบ) เนื่อจากการหยุดใช้พลังงานอย่างกระทันหัน
      จากการเดินทางในประเทศและต่างประเทศ รวมไปถึงการหยุดบริโภคพลังงานอุตสาหกรรมหนักขนาดใหญ่และครัวเรือน

    #### <u>Next Action Plan</u>
    - หากเกิดเหตุการณ์ที่มีการปรับตัวราคาสินค้าลงอย่างรุนแรงให้อย่ารีบขายสินทรัพย์ที่มีอยู่ เนื่องจากราคาสินค้าจะปรับตัวสู่สภาวะปกติในเวลาถัดมา
    - ในช่วงที่ราคาสินค้าราคาต่ำจากวิกฤตการณ์อาจะเป็นโอกาศในการบริโภคสินค้าราคาถูก การแบ่งลงทุนในช่วงนี้จึงอาจจะเป็นโอกาศที่ดีในการลงทุน
    - การกระจายความเสี่ยงโดยแบ่งลงทุนในสินทรัพย์ทองคำ ซึ่งเป็น"โลหะมีค่า"
    
    
   
2. กลุ่มของสินค้าโภคภัณฑ์กลุ่มใดได้รับหรือเสียประโยชน์จากสถานะการณ์Covid-19 อย่างไร ?

    - ??

4. ข้อสรุปที่ได้นอกเหนือจากการตั้งคำถามตอนแรก คือ
    - สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์มีราคาที่ปรับตัวสูงขึ้นค่อนข้างคงที่ตั้งแต่ช่วงเริ่มต้นการระบาดของCovid-19 จนถึงปัจจุบันโดยไม่สัมพันธ์กัน
      จำนวนผู้ติดเชื้อCovid-19 แสดงให้เห็นว่าต้องมีปัจจัยอื่นที่ส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ประเภทนี้

    #### <u>Next Action Plan</u>
    - แนวโน้มสินค้าโภคภัณฑ์ประเภทอาหารซึ่งเป็นปัจจัย4มีทิศทางสูงขึ้นเรื่อยๆ จึงมีความจำเป็นต้องหารายได้ให้มากขึ้นในอนาคตเพื่อความอยู่รอด


               
## Reference
  - https://th.investing.com/commodities/ (ราคาสินค้าโภคภัณฑ์)
  - https://covid19.who.int/data  (จำนวนยอดผู้ติดเชื้อโควิดทั่วโลก)




