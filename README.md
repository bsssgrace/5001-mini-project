# Covid-19 Situation Impact on Commodity prices
![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

## Hypothesis
1.Commodity ทีราคาผันผวนในช่วงโควิดที่ผ่านมาความสัมพันธ์ ราคาส่งผลกระทบมาจาก Covid new case มากแค่ไหน
2.

[Grace] คาดว่าจำนวนผู้ติดเชื้อโควิดตั้งแต่เริ่มมีการประกาศภาวะฉุกเฉินในเดือนมกราคม ปี 2563 เป็นต้นมา ส่งผลต่อราคาผันผวนของสินค้าโภคภัณฑ์ในตลาดโลก เนื่องจากปัจจัยในการส่งออก-นำเข้า, กำลังการผลิต หรือ ความต้องการใช้สินค้าโภคภัณฑ์ในแต่ละประเภท เป็นต้น
ดังนั้น EDA ที่จะนำเสนอต่อไปนี้ จึงเป็นการวิเคราะห์จากราคาสินค้าโภคภัณฑ์ในแต่ละประเภทควบคู่ไปกับจำนวนผู้ติดเชื้อโควิดรายวันทั่วโลก เพื่อให้เห็นถึงความสัมพันธ์ของ 2 ข้อมูลดังกล่าว ......
  
### ศึกษาผลกระทบของสินค้าโภคภัณฑ์จากการะบาดของโควิด-19 [Grace]ประเภทของสินค้าโภคภัณฑ์... เพิ่มอีก ## อธิาบเรื่องการแบ่งช่วงสีแดงในแต่ละช่วง --> definition คืออะไร
โดยเราทำการแบ่งกลุ่มของสินค้าโภคภัณฑ์เป็น 4 ประเภท
- 1.สินค้าประเภทพลังงาน [Grace] ได้แก่ (subset ของ Energy) [Boss] ได้แก่ น้ำมันดิบ, ก๊าซธรรมชาติ, น้ำมันให้ความร้อน และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้เป็นสินค้าที่มีปริมาณความต้องการเป็นจำนวนมาก เพราะ เป็นปัจจัยสำคัญต่อระบบขนส่งทั่วโลก และยังเป็นสินค้าหลักในการผลิดพลังงานและความร้อนแก่อุตสาหกรรมและบ้านเรือน
- 2.สินค้าประเภทโลหะ [Boss] ได่แก่ ดีบุก, ตะกั่ว, อะลุมิเนียม, เงิน, ทองคำ, นิกเกิล, สังกะสี, พาลาเดียม และ อื่นๆ
  - สินค้าโภคภัณฑ์ประเภทนี้ใช้เป็นวัตถุดิบในหลายอุตสาหกรรมหนัก ไม่ว่าจะเป็นอุตสาหกรรมเครื่องใช้ไฟฟ้าหรืออุปกรณ์อิเล็กทรอนิกส์จนไปถึงอุตสาหกรรมเพื่อความงาม และบางสินค้าอย่างเช่นทองคำ ยังอยู่ในกลุ่มของ "โลหะมีค่า" (Precious        Metal) เพื่อการลงทุนในระยะยาวอีกด้วย 
- 3.สินค้าประเภทเนื้อสัตว์ [Boss] ได่แก่ 
- 4.สินค้าประเภทการเกษตร (same) ได้แก่ กาแฟ, โกโก้, ไม่แปรรูป, น้ำตาล, น้ำส้ม และอื่นๆ
  - สินค้าประเภท Soft commodity หรือผลิตภัณฑ์จากการเพราะปลูกจะมีอายุเก็บรักษาที่จำกัดไม่สามารถเก็บได้ไว้นานซึ่งมีความผันผวนของราคาค่อนข้างสูงเนื่องจากปัจจั 
    เสี่ยงที่ไม่สามารถคุมได้อาทิ สภาพอากาศ, ปริมาณน้ำ เป็นต้น
- 5.สินค้าประเภทเมล็ดพืช [Boss] ได้แก่ ข้าวสาลี, ข้าวโอต, ข้าวโพด, ถั่วเหลือง, น้ำมันถั่วเหลือง และ อื่นๆ
  - สินค้าประเภทนี้เป็นสินค้าที่สามารถบริโภคได้ด้วยตรงและเป็นสินค้าที่สามารถเป็นผลิตภัณฑ์แปรรูปได้อาทิ แป้งข้าวโพด, ขนมปัง เพื่อเป็นการบริโภคทางอ้อม รวมไปถึงเป็นอาหารของสัตว์ที่จำถูกนำมาบริโภคในลำดับถัดๆไป
### 1.สินค้าประเภทพลังงาน

![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

  ข้อสรุป
  - 1.การหยุดใช้พลังงานอย่างกระทันหันเนืองจาก พลังงานจากการเดินทางในประเทศและต่างประเทศ, การหยุดบริโภคพลังงานจากโรงงาน
  - 2.หลังจากเริ่มเปิดประเทศในช่วงนี้ Q4 2021 ราคาน้ำมันทุกประเภทเริ่มค่อยๆฟื้นตัวตอนเริ่มเปิดประเทศ จนไปถึงช่วงที่การท่องเที่ยวเริ่มฟื้นตัวจากมาตรการผ่อนคลายการท่องเที่ยว
  - 

### 2. สินค้าประเภทโลหะ
![metal](https://github.com/bsssgrace/5001-mini-project/assets/114140787/cf81e1c7-e15a-4ce3-a478-4cd06623f2f3)

(กราฟ)

  ข้อสรุป
  - ราคาโลหะไม่ได้มีความสัมพันธ์กับอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื่อโควิด
  - การลดจำนวนผู้ติดเชื้อไม่ได้ช่วยให้ลดความผันผวนของราคาโลหะ
  - ราคาโลหะที่ผันผวน ไม่สามารถอธิบายได้ด้วยจำนวนผู้ติดเชื่อโควิด อาจจะต้องหาปัจจัยอื่นมาอธิบายเพิ่มเติม
  - 

### 3.สินค้าประเภทเนื้อสัตว์
![meat](https://github.com/bsssgrace/5001-mini-project/assets/114140787/63a1a9f9-f8eb-40a6-889a-1a1d173630ee)


  ข้อสรุป
  - ฟหกด
  - ก

### 4. สินค้าประเภทการเกษตร

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/e2722d68-8b64-4170-bfe1-71289e538451)


  ข้อสรุป
  - ฟหกด
  - ก




### 5. สินค้าประเภทเมล็ดพืช

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/8951642b-ca9d-430d-9628-a82b070bc5b0)

  ข้อสรุป
  - ฟหกด
  - ก

# Summary
ข้อสรุป
1.ผลกระทบของโควิด Impact ราคาโภคภัณฑ์ในช่วงแรกทำให้ราคาตกลงในช่วงต้น(ราคาข้าวเปลือก) จนถึงปลายq1ของ2020
2.หลังจากปลายq1ของ2020 เริ่มไม่เห็นความสัมพันธ์สินค้าโภคภัณฑ์กับจำนวนผู้ติดเชื้อ
3.ไม่เกี่ยวกับโควิด - หลายสินค้าส่วนใหญ่มีราคามีผันผวนจากปัจจัยอื่นที่ไม่ใช่โควิด เช่น การหยุดส่งออกข้าวของผู้ผลิตรายใหญ่ 
  เกี่ยวกับโควิด - บางสินค้าก็มีราคาที่ผันผวนโดยได้รับผลกระทบจากโควิดในช่วงต้น เช่น การหยุดใช้พลังงานอย่างกระทันหันเนืองจาก พลังงานจากการเดินทางในประเทศและต่างประเทศ, การหยุดบริโภคพลังงานจาก 
               โรงงาน 
               
# Reference
  - https://th.investing.com/commodities/ (ราคาสินค้าโภคภัณฑ์)
  - https://covid19.who.int/data  (จำนวนยอดผู้ติดเชื้อโควิดทั่วโลก)




