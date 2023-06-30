# Covid-19 Situation Impact on Commodity prices
![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

## Background
    
จากสถานการณ์ Covid-19 โควิดเป็นโรคติดต่อระบาดครั้งใหญ่ของโลก โดยเป็นโรคติดต่อร้ายแรงที่เกิดขึ้นมาใหม่ในเมืองอู่ฮั่นที่ประเทศจีนเมื่อเดือนธันวาคม ปี 2019 
ไวรัสชนิดนี้เป็นชนิดใหม่ที่ไม่เคยพบเจอที่ไหนมาก่อน เป็นโรคภัยพิบัติที่ทำให้เกิดความวิตกกังวลอย่างมากต่อชีวิตของคนทั่วโลกมาจนถึงปัจจุบัน 

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/bbb89762-1753-4abc-a80e-514389032ba9)

จากกราฟด้านบน เราแบ่ง Timeline ของสถานการณ์โควิดออกเป็น 5 ช่วงหลักๆ คือ
- 1.ช่วงค้นพบโรค Covid-19 และ เริ่มระบาดทั่วโลก
- 2.ช่วงของการปิดประเทศและการกักตัวตามนโยบายควบคุมโรคในแต่ละประเทศ
- 3.ช่วงเริ่มต้นของการผ่อนคลายและเริ่มเปิดเขตแดนระหว่างประเทศ
- 4.ช่วงที่ประกาศ Covid-19 เป็นเชื้อโรคประจำถิ่นและเปิดให้มีกิจกรรมสันทนาการ
- 5.ช่วงที่ประเทศจีนเริ่มผ่อนคลายนโยบาย Zero-Covid Policy จึงมีผู้ติดเชื้อเพิ่มขึ้นเป็นจำนวนมาก ประกอบกับการรวบรวมตัวเลขผู้ติดเชื้อที่ล่าช้า ทำให้การรายงานผู้ติดเชื้อพุ่งสูงเกินความเป็นจริงในระยะเวลาสั้นๆ และตกลงอย่างรวดเร็ว ซึ่งแตกต่างจากช่วงอื่นๆ ที่มีการรายงานผู้ติดเชื้ออย่างต่อเนื่อง ประกอบกับช่วงเวลาที่ผ่านมาเกิดสภาวะตลาดสินค้าโภคภัณฑ์ที่มีการปรับตัวของราคาสินค้าอย่างผันผวน เราจึงเริ่มตั้งคำถามในสิ่งที่เราสนใจ

## คำถามที่เกิดขึ้น
- 1.สถานการณ์การระบาดของ Covid-19 ทั่วโลกส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ในปัจจุบันมากหรือน้อยเพียงใด ?
- 2.กลุ่มของสินค้าโภคภัณฑ์กลุ่มใด ได้รับหรือเสียประโยชน์จากสถานการณ์ Covid-19 ?
  
## เราทำการแบ่งกลุ่มของสินค้าโภคภัณฑ์หลักเป็น 5 ประเภท 
- `1.สินค้าโภคภัณฑ์ประเภทพลังงาน`
  - ได้แก่ น้ำมันดิบ, ก๊าซธรรมชาติ, น้ำมันให้ความร้อน
  - สินค้าโภคภัณฑ์ประเภทนี้เป็นสินค้าที่มีปริมาณความต้องการเป็นจำนวนมาก เพราะเป็นปัจจัยสำคัญต่อระบบขนส่งขนาดใหญ่ทั่วโลก และยังเป็นสินค้าหลักในการผลิตพลังงานและความร้อนแก่อุตสาหกรรมหนักขนาดใหญ่และครัวเรือน
    
- `2.สินค้าโภคภัณฑ์ประเภทโลหะ`
  - ได้แก่ ดีบุก, ตะกั่ว, อะลูมิเนียม, เงิน, ทองคำ, นิกเกิล, สังกะสี, พาลาเดียม
  - สินค้าโภคภัณฑ์ประเภทนี้ใช้เป็นวัตถุดิบในหลายอุตสาหกรรมหนัก ไม่ว่าจะเป็นอุตสาหกรรมเครื่องใช้ไฟฟ้าหรืออุปกรณ์อิเล็กทรอนิกส์จนไปถึงอุตสาหกรรมเครื่องประดับ และบางสินค้าอย่างเช่น ทองคำ ยังอยู่ในกลุ่มของ "โลหะมีค่า" (Precious Metal) เพื่อการลงทุนในระยะยาวอีกด้วย
    
- `3.สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์`
  - ได้แก่ เนื้อหมู, เนื้อวัว
  - สินค้าประเภทนี้เป็นเนื้อสัตว์เพื่อการบริโภค
   
- `4.สินค้าโภคภัณฑ์จากการเพาะปลูกที่ไม่ใช่เมล็ดพืช`
  - ได้แก่ กาแฟ, โกโก้, ไม่แปรรูป, น้ำตาล, น้ำส้ม
  - สินค้าประเภทการเกษตรเป็น Soft commodity หรือผลิตภัณฑ์จากการเพราะปลูก จะมีอายุเก็บรักษาที่จำกัดและไม่สามารถเก็บไว้ได้นาน ซึ่งมีความผันผวนของราคาค่อนข้างสูงเนื่องจากปัจจัยเสี่ยงที่ไม่สามารถควบคุมได้ อาทิ สภาพอากาศและปริมาณน้ำ เป็นต้น
     
- `5.สินค้าโภคภัณฑ์ประเภทธัญพืช`
  - ได้แก่ ข้าวสาลี, ข้าวโอ๊ต, ข้าวโพด, ถั่วเหลือง, น้ำมันถั่วเหลือง
  - สินค้าประเภทนี้เป็นสินค้าที่บริโภคได้โดยตรงและสามารถแปรรูปได้ อาทิ แป้งข้าวโพด, ขนมปัง รวมไปถึงเป็นอาหารของสัตว์

## การเปลี่ยนแปลงข้อมูลราคาโภคภัณฑ์ (Data Transformation) เพื่อให้สามารถเปรียบเทียบกันได้
- เนื่องจากราคาสินค้าแต่ละประเภทมีช่วงค่าที่แตกต่างกันเยอะมาก เช่น ราคาสินค้าประเภทหนึ่งมีราคาตั้งแต่ 100 - 1,000 ในขณะที่สินค้าอีกประเภทมีราคา 10,000 - 1,000,000 หากนำมาแสดงผลในกราฟเดียวกัน จะทำให้ไม่เห็นความแตกต่างของราคาที่มีช่วงเล็กกว่า เราจึงต้อง normalize ให้สามารถเปรียบเทียบกันได้
- วิธีการคือใช้สูตร (Price_at_date - Min_Price) / (Max_Price - Min_Price) ซึ่งจะมีค่าอยู่ระหว่าง 0 ถึง 1 เสมอ โดยตั้งชื่อ Field ที่คำนวณขึ้นมาใหม่นี้ว่า Norm_Price

## กราฟแสดงราคาสินค้าโภคภัณฑ์แต่ละประเภทเพื่อหาข้อสรุป
### 1.สินค้าโภคภัณฑ์ประเภทพลังงาน

![energy](https://github.com/bsssgrace/5001-mini-project/assets/114140787/56441409-ee52-470d-a8fa-41b8c24e0c69)

![Crude Oil (WTI) vs COVID Cases](https://github.com/bsssgrace/5001-mini-project/assets/16522923/161eef64-d586-4bac-9319-78446dbf86a1)

  ข้อสรุป
  - ราคาสินค้าพลังงานทุกประเภทตกลงอย่างมากในช่วงเริ่มระบาดของโควิด สาเหตุมาจากการหยุดใช้พลังงานอย่างกระทันหันจากการระงับการเดินทางทั้งในและต่างประเทศ และการลดการใช้พลังงานของภาคธุรกิจและภาคอุตสาหกรรม
  - ปัจจัยเสริมฝั่งผู้ผลิต ไม่สามารถปรับลดปริมาณการผลิตลงมาได้ทันกับอุปสงค์ที่ลดลงกระทันหัน ทำให้ราคาน้ำมันดิบมีราคาติดลบในช่วงเวลาหนึ่ง เนื่องจากค่าใช้จ่ายในการเก็บรักษาสต็อกที่ล้น มากกว่าค่าใช้จ่ายในการแจกจ่ายออกโดยไม่คิดราคา
  - ราคาสินค้าพลังงานเริ่มฟื้นตัวหลังจากผ่านช่วงเริ่มต้นของโควิด และปรับตัวสูงขึ้นอีกในช่วงเริ่มเปิดประเทศตั้งแต่ไตรมาส 4 ปี 2021 ไปจนถึงการผ่อนคลายควบคุมการท่องเที่ยวและกิจกรรมสันทนาการ
  - ราคาสินค้าพลังงานค่อยๆ ปรับตัวลดลงหลังจากช่วงผ่อนคลายควบคุมการท่องเที่ยวและกิจกรรมสันทนาการ จนกลับมาในระดับเดียวกับราคาก่อนโควิด
    
### 2. สินค้าโภคภัณฑ์ประเภทโลหะ

![metal](https://github.com/bsssgrace/5001-mini-project/assets/114140787/cf81e1c7-e15a-4ce3-a478-4cd06623f2f3)

  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์ประเภทโลหะทุกประเภทมีราคาตกในช่วงแรกที่เกิด Covid-19 (ช่วงมีนาคม 2020)
  - ราคาสินค้าโภคภัณฑ์ประเภทโลหะหลังจากช่วงแรกของโควิดไม่ได้มีความสัมพันธ์อย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื้อโควิด หากต้องการอธิบายความผันผวนจะต้องใช้ปัจจัยอื่นมาอธิบาย

### 3.สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์

![meat](https://github.com/bsssgrace/5001-mini-project/assets/114140787/63a1a9f9-f8eb-40a6-889a-1a1d173630ee)

  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์ประเภทเนื้อสัตว์ทุกประเภทมีราคาตกในช่วงแรกที่เกิด Covid-19 (ช่วงมีนาคม 2020)
  - จากกราฟจะสังเกตเห็นว่า ราคาเนื้อสัตว์ที่พร้อมสำหรับบริโภค (Live Cattle, Live Hogs)O มีแนวโน้มราคาที่ปรับตัวสูงขึ้นอยู่ตลอด ไม่ได้สัมพันธ์กับจำนวนยอดผู้ติดเชื้อโควิด จะต้องใช้ปัจจัยอื่นมาอธิบาย

### 4. สินค้าโภคภัณฑ์จากการเพาะปลูกที่ไม่ใช่เมล็ดพืช

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/e2722d68-8b64-4170-bfe1-71289e538451)

  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์จากการเพาะปลูกที่ไม่ใช่เมล็ดพืชทุกประเภทมีราคาตกในช่วงแรกที่เกิด Covid-19 (ช่วงมีนาคม 2020)
  - ราคาสินค้าโภคภัณฑ์ประเภทการเกษตรไม่ได้มีความสัมพันธ์กันอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื้อโควิด ต้องใช้ปัจจัยอื่นมาอธิบายเพิ่มเติม

### 5. สินค้าโภคภัณฑ์ประเภทธัญพืช

![image](https://github.com/bsssgrace/5001-mini-project/assets/117662533/8951642b-ca9d-430d-9628-a82b070bc5b0)

  ข้อสรุป
  - ราคาสินค้าโภคภัณฑ์ประเภทธัญพืชมีราคาตกในช่วงแรกที่เกิด Covid-19 (ช่วงมีนาคม 2020) ยกเว้นข้าวเปลือกที่มีราคาขึ้นสูง ก่อนจะตกลงมาใกล้เคียงกับสินค้าธัญพืชอื่นๆ
  - ราคาข้าวเปลือกมีราคาที่สูงขึ้นอย่างโดดเด่นในช่วงไตรมาส 1-2 ของปี 2020 เนื่องจากการกักตุนสินค้าของผู้ผลิตรายใหญ่อย่างเวียดนาม
  - ราคาสินค้าโภคภัณฑ์ประเภทธัญพืชไม่ได้มีความสัมพันธ์กันอย่างมีนัยยะสำคัญกับจำนวนผู้ติดเชื้อโควิด ต้องหาปัจจัยอื่นมาอธิบายเพิ่มเติม

## Overall Summary & Possible Actions from Insights

1. สถานการณ์การระบาดของ Covid-19 ทั่วโลกส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ในปัจจุบันมากหรือน้อยเพียงใด ?
    - ผลกระทบจากสถานการณ์ Covid-19 ทำให้สินค้าโภคภัณฑ์ทุกประเภทมีราคาตกลงอย่างเห็นได้ชัดในช่วงแรกของการระบาดเป็นช่วงสั้นๆ จากนั้นราคาปรับตัวขึ้นมาในระดับก่อนโควิดและมีความเปลี่ยนแปลงโดยไม่มีความสัมพันธ์กับจำนวนผู้ติดเชื้ออย่างมีนัยยะสำคัญ
    - สินค้าโภคภัณฑ์ที่ได้รับผลกระทบอย่างหนักที่สุดในช่วงแรกของการระบาด คือ น้ำมันดิบ (ลดลงจนติดลบ) เนื่องจากการหยุดใช้พลังงานอย่างกระทันหัน จากการระงับเดินทางในประเทศและต่างประเทศ และการลดการใช้พลังงานของภาคธุรกิจและภาคอุตสาหกรรม ประกอบกับผู้ผลิตน้ำมันดิบปรับกำลังการผลิตลงไม่ทัน ส่งผลให้น้ำมันดิบล้นตลาด

2. กลุ่มของสินค้าโภคภัณฑ์กลุ่มใดได้รับหรือเสียประโยชน์จากสถานะการณ์Covid-19 อย่างไร ?
    - สินค้าโภคภัณฑ์ทุกกลุ่มเสียประโยชน์จากราคาสินค้าที่ตกลงในช่วงแรกในการระบาดของ Covid-19 โดยเฉพาะน้ำมันดิบ (Crude Oil) ซึ่งผู้ผลิดไม่ยอมลดกำลังการผลิตแม้ว่าจะมีปัจจัยทำให้อุปสงต์ตกอย่างรุนแรง

## <u>Possible Actions from Insights</u> ##
    - สำหรับผู้ผลิตหรือผู้ขายสินค้าโภคภัณฑ์ หากเกิดเหตุการณ์ที่ราคาสินค้าของตนตกลงอย่างกระทันหันจากวิกฤตการณ์ที่ไม่คาดคิด (Black Swan Event) ให้พยายามขายสินค้าที่มีอยู่ให้น้อยที่สุดเพื่อลดการขาดทุน เนื่องจากราคาสินค้าจะปรับตัวสู่สภาวะปกติในเวลาถัดมา
    - สำหรับผู้ซื้อสินค้าโภคภัณฑ์ ในช่วงที่ราคาสินค้าราคาต่ำจากวิกฤตการณ์ดังกล่าว อาจจะเป็นโอกาสในการซื้อสินค้าโภคภัณฑ์ราคาถูกกว่าราคาปกติ
    
3. ข้อสรุปที่ได้นอกเหนือจากการตั้งคำถามตอนแรก คือ
    - สินค้าโภคภัณฑ์ประเภทเนื้อสัตว์มีราคาที่ปรับตัวสูงขึ้นค่อนข้างคงที่ตั้งแต่ช่วงเริ่มต้นการระบาดของ Covid-19 จนถึงปัจจุบันโดยไม่สัมพันธ์กับจำนวนผู้ติดเชื้อ Covid-19 แสดงให้เห็นว่าต้องมีปัจจัยอื่นที่ส่งผลกระทบต่อราคาสินค้าโภคภัณฑ์ประเภทนี้
    - <b>สินค้าโภคภัณฑ์เป็นสินค้าที่ได้รับผลกระทบน้อยจากวิกฤตการณ์ที่ไม่คาดคิด (Black Swan Event)</b> เนื่องจากเป็นปัจจัยพื้นฐานในวิถีชีวิตของมนุษย์ทั่วโลก เมื่อเทียบกับผลิตภัณฑ์หรือบริการอื่นๆ ที่ได้รับผลกระทบอย่างมาก เช่น อุตสาหกรรมเทคโนโลยี หรือ Cryptocurrency

## <u>Possible Actions from Insights</u> ##
    - การเลือกทำธุรกิจที่เกี่ยวข้องกับโภคภัณฑ์ถือเป็นหนึ่งในทางเลือกที่น่าสนใจของผู้ต้องการลงทุนในธุรกิจ เนื่องจากได้รับผลกระทบน้อยจากจากวิกฤตการณ์ที่ไม่คาดคิด (Black Swan Event) 
    อย่างไรก็ตามสินค้าโภคภัณฑ์เป็นสินค้าที่มีราคาผันผวนเป็นปกติ และผู้ผลิตไม่สามารถสร้างแบรนด์หรือสร้างความแตกต่างจากคู่แข่งได้อย่างชัดเจน จึงไม่สามารถควบคุมราคาสินค้าของตนได้ 
    ผู้ต้องการลงทุนในธุรกิจโภคภัณฑ์จะต้องตระหนักในปัจจัยทั้งด้านบวกและลบก่อนตัดสินใจลงทุน
               
## Reference
  - https://th.investing.com/commodities/ (ราคาสินค้าโภคภัณฑ์)
  - https://covid19.who.int/data  (จำนวนยอดผู้ติดเชื้อโควิดทั่วโลก)
