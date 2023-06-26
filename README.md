# Covid-19 Situation Impact on Commodity prices
![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

## Hypothesis
1.สถานะการ์การระบาดของCovid-19ทั่วโลกส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ในปัจจุบันมากเพียงใด
2.กลุ่มของสินค้าโภคภัณฑ์แต่ละชนิดได้รับผลกระทบจากสถานะการณ์Covid-19มากน้อยอย่างไร

[Grace] คาดว่าจำนวนผู้ติดเชื้อโควิดตั้งแต่เริ่มมีการประกาศภาวะฉุกเฉินในเดือนมกราคม ปี 2563 เป็นต้นมา ส่งผลต่อราคาผันผวนของสินค้าโภคภัณฑ์ในตลาดโลก เนื่องจากปัจจัยในการส่งออก-นำเข้า, กำลังการผลิต หรือ ความต้องการใช้สินค้าโภคภัณฑ์ในแต่ละประเภท เป็นต้น
ดังนั้น EDA ที่จะนำเสนอต่อไปนี้ จึงเป็นการวิเคราะห์จากราคาสินค้าโภคภัณฑ์ในแต่ละประเภทควบคู่ไปกับจำนวนผู้ติดเชื้อโควิดรายวันทั่วโลก เพื่อให้เห็นถึงความสัมพันธ์ของ 2 ข้อมูลดังกล่าว ......
  
### ศึกษาผลกระทบของสินค้าโภคภัณฑ์จากการะบาดของโควิด-19 [Grace]ประเภทของสินค้าโภคภัณฑ์... เพิ่มอีก ## อธิาบเรื่องการแบ่งช่วงสีแดงในแต่ละช่วง --> definition คืออะไร
#### โดยเราทำการแบ่งกลุ่มของสินค้าโภคภัณฑ์เป็น 4 ประเภท
- `1.สินค้าประเภทพลังงาน`
  - [Grace] ได้แก่ (subset ของ Energy) [Boss] ได้แก่ น้ำมันดิบ, ก๊าซธรรมชาติ, น้ำมันให้ความร้อน และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้เป็นสินค้าที่มีปริมาณความต้องการเป็นจำนวนมาก เพราะ เป็นปัจจัยสำคัญต่อระบบขนส่งขนาดใหญ่ทั่วโลก และยังเป็นสินค้าหลักในการผลิด 
    พลังงานและความร้อนแก่อุตสาหกรรมหนักขนาดใหญ่และครัวเรือน
    
- `2.สินค้าประเภทโลหะ`
  - [Boss] ได้แก่ ดีบุก, ตะกั่ว, อะลุมิเนียม, เงิน, ทองคำ, นิกเกิล, สังกะสี, พาลาเดียม และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้ใช้เป็นวัตถุดิบในหลายอุตสาหกรรมหนัก ไม่ว่าจะเป็นอุตสาหกรรมเครื่องใช้ไฟฟ้าหรืออุปกรณ์อิเล็กทรอนิกส์จนไปถึงอุตสาหกรรมเพื่อความงาม  
    และบางสินค้าอย่างเช่นทองคำ ยังอยู่ในกลุ่มของ "โลหะมีค่า" (Precious Metal) เพื่อการลงทุนในระยะยาวอีกด้วย
    
- `3.สินค้าประเภทเนื้อสัตว์`
  - [Boss] ได้แก่ เนื้อหมู, เนื้อวัว, เนื้อไก่ และ อื่นๆ
  - สินค้าประเภทนี้อาจจะดูคล้ายกับสินค้าทางการเกษตรแต่สินค้าที่มาจากสัตว์เพื่อการบริโภค
   
- `4.สินค้าประเภทการเกษตร`
  - [Boss] ได้แก่ กาแฟ, โกโก้, ไม่แปรรูป, น้ำตาล, น้ำส้ม และอื่นๆ
  - สินค้าประเภท Soft commodity หรือผลิตภัณฑ์จากการเพราะปลูกจะมีอายุเก็บรักษาที่จำกัดไม่สามารถเก็บได้ไว้นานซึ่งมีความผันผวนของราคาค่อนข้างสูงเนื่องจาก 
    ปัจจัยเสี่ยงที่ไม่สามารถคุมได้อาทิ สภาพอากาศ, ปริมาณน้ำ เป็นต้น
     
- `5.สินค้าประเภทเมล็ดพืช`
  - [Boss] ได้แก่ ข้าวสาลี, ข้าวโอต, ข้าวโพด, ถั่วเหลือง, น้ำมันถั่วเหลือง และ อื่นๆ
  - สินค้าประเภทนี้เป็นสินค้าที่สามารถบริโภคได้ด้วยตรงและเป็นสินค้าที่สามารถเป็นผลิตภัณฑ์แปรรูปได้อาทิ แป้งข้าวโพด, ขนมปัง เพื่อเป็นการบริโภคทางอ้อม        
    รวมไปถึงเป็นอาหารของสัตว์ที่จำถูกนำมาบริโภคในลำดับถัดๆไป


### 1.โภคภัณฑ์ประเภทพลังงาน

![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

  ข้อสรุป
  - 1.การหยุดใช้พลังงานอย่างกระทันหันเนืองจาก พลังงานจากการเดินทางในประเทศและต่างประเทศ, การหยุดบริโภคพลังงานจากโรงงาน
  - 2.หลังจากเริ่มเปิดประเทศในช่วงนี้ Q4 2021 ราคาน้ำมันทุกประเภทเริ่มค่อยๆฟื้นตัวตอนเริ่มเปิดประเทศ จนไปถึงช่วงที่การท่องเที่ยวเริ่มฟื้นตัวจากมาตรการผ่อนคลายการท่องเที่ยว
  - 

### 2. โภคภัณฑ์ประเภทโลหะ

![metal](https://github.com/bsssgrace/5001-mini-project/assets/114140787/cf81e1c7-e15a-4ce3-a478-4cd06623f2f3)

  ข้อสรุป
  - ราคาโลหะไม่ได้มีความสัมพันธ์กับอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื่อโควิด
  - ทองคำเป็นสินค้าเพื่อการลงทุนและนิยมซื้อเก็บเพื่อรักษาความเสี่ยงทางการเงินที่ราคาปรับตัวสูงขึ้นอย่างโดดเด่นเนื่องจากสถานะการโควิด
  - การลดจำนวนผู้ติดเชื้อไม่ได้ช่วยให้ลดความผันผวนของราคาโลหะ
  - ราคาโลหะที่ผันผวน ไม่สามารถอธิบายได้ด้วยจำนวนผู้ติดเชื่อโควิด อาจจะต้องหาปัจจัยอื่นมาอธิบายเพิ่มเติม

  - 
### 3.โภคภัณฑ์ประเภทเนื้อสัตว์

![meat](https://github.com/bsssgrace/5001-mini-project/assets/114140787/63a1a9f9-f8eb-40a6-889a-1a1d173630ee)

  ข้อสรุป
  - จากกราฟจะสังเกตุเห็นว่าราคาเนื้อสัตว์(เนื้อหมู,เนื้อวัว)ที่พร้อมสำหรับบริโภคมีแนวโน้มราคาที่ปรับตัวสูงขึ้นอยู่ตลอดไม่ได้สัมพันธ์กับจำนวนยอดผู้ติดเชื้อโควิด ซึ่งราคาที่ 
    ปรับตัวขึ้นของสินค้าประเภทนี้น่าจะมาจากปัยจัยอื่นเช่นอัตราเงินเฟ้อ โดยทำให้เราสามารถตัดปัจจัยจากยอดผู้ติดเชื่อโควิดได้ 

### 4. โภคภัณฑ์ประเภทการเกษตร

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/e2722d68-8b64-4170-bfe1-71289e538451)


  ข้อสรุป
  - ?
  - 




### 5. โภคภัณฑ์ประเภทเมล็ดพืช

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/8951642b-ca9d-430d-9628-a82b070bc5b0)

  #### ข้อสรุป
  - โภคภัณฑ์ประเภทนี้มีการปรับราคาโดยรวมสูงขึ้นไปในทางเดียวกันกับโภคภัณฑ์ประเภทเนื้อสัตว์โดยราคาปัจจุบันยังไม่สามารถกลับไปในช่วงก่อนเกิดสถานการณ์โควิดได้
  - ราคาข้าวเปลือกมีราคาที่สูงขึ้นอย่างโดดเด่นในช่วงไตรมาส1-2 ของปี 2020 อย่างโดดเด่น แต่เมื่อทำการค้นหาข้อมูลเพิ่มพบปัจจัยราคาที่สูงขึ้นเกิดการ 
    กักตุนสินค้าจากผู้ผลิตรายใหญ่อย่างเวียดนาม (ไม่ได้เ้กี่ยวข้องกับสถานะการCovid-19แต่อย่างใด)

## Summary
  ข้อสรุป
  - 1.ผลกระทบจากสถานะการCovid-19 มีผลทำให้ทุกสินค้าโภคภัณฑ์มีราคาที่ต่ำลงอย่างเห็นได้ชัดในช่วงแรกของการระบาดและ                            
      ราคาสินค้าเริ่มฟื้นตัวกลับสู่ราคาเดิมหรือมากกว่าก่อนเกิดการระบาดของCovid-19
  - 2.สินค้าโภคภัณฑ์ที่ได้รับผลกระทบอย่างชัดเจนในช่วงแรกของการระบาดคือราคาน้ำมัน(ติดลบ) เนื่อจากการหยุดใช้พลังงานอย่างกระทันหัน
      จากการเดินทางในประเทศและต่างประเทศ รวมไปถึงการหยุดบริโภคพลังงานอุตสาหกรรมหนักขนาดใหญ่และครัวเรือน
  - 3.สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์มีราคาที่ปรับตัวสูงขึ้นค่อนข้างคงที่ตั้งแต่ช่วงเริ่มต้นการระบาดของCovid-19 จนถึงปัจจุบันโดยไม่สัมพันธ์กัน
      จำนวนผู้ติดเชื้อCovid-19 แสดงให้เห็นว่าต้องมีปัจจัยอื่นที่ส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ประเภทนี้
    
               
***Reference***
  - https://th.investing.com/commodities/ (ราคาสินค้าโภคภัณฑ์)
  - https://covid19.who.int/data  (จำนวนยอดผู้ติดเชื้อโควิดทั่วโลก)




