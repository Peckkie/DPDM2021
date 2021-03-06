Week 2 / SC637802 Data Pre-processing and Data Mining

By YUPAPORN WANNA 645020061-2
 
---
# บทที่ 2: การทำความเข้าใจข้อมูล (Getting to Know Your Data) 
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#ประเภทของข้อมูล">ประเภทของข้อมูล</a></li>
    <li><a href="#ลักษณะสำคัญของโครงสร้างข้อมูล">ลักษณะสำคัญของโครงสร้างข้อมูล</a></li>
    <li><a href="#Data-Objects-and-Attribute-Types">Data Objects and Attribute Types</a></li> 
    <li><a href="#Measuring-Data-Similarity-and-Dissimilarity">Measuring Data Similarity and Dissimilarity</a></li> 
  </ol>
</details>

## Data Objects and Attribute Types
### ประเภทของข้อมูล 
"ประเภทของข้อมูล (Types of Data Sets)"

(1) Record Data
> - Relational records
<br /><p align="left"><a><img src="img/Chapter2_0.jpg" alt="Logo" width="600" ></a> </p><br />
> - Data matrix, e.g., numerical matrix, crosstabs
<br /><p align="left"><a><img src="img/Chapter2_1.jpg" alt="Logo" width="600" ></a> </p><br />
> - Transaction data
<br /><p align="left"><a><img src="img/Chapter2_2.jpg" alt="Logo" width="600" ></a> </p><br />
> - Document data: Term-frequency vector (matrix) of text documents
<br /><p align="left"><a><img src="img/Chapter2_3.jpg" alt="Logo" width="600" ></a> </p><br />

(2) ประเภทข้อมูลที่เป็นกราฟเเละเคลือข่าย (Graphs and Networks)
> <br /><p align="center"><a><img src="img/Chapter2_4.jpg" alt="Logo" width="900" ></a> </p><br />

(3) ประเภทข้อมูลที่เป็นอันดับหรือลำดับเเละลำดับของข้อมูลมีความสำคัญ (Ordered Data)
> <br /><p align="center"><a><img src="img/Chapter2_5.jpg" alt="Logo" width="900" ></a> </p><br />

(4) ประเภทข้อมูลลักษณธเชิงพื้นที่ รูปภาพ เเละวิดีโอ (Spatial, image and multimedia Data)
> <br /><p align="center"><a><img src="img/Chapter2_6.jpg" alt="Logo" width="900" ></a> </p><br />

### ลักษณะสำคัญของโครงสร้างข้อมูล
"ลักษณะสำคัญของโครงสร้างข้อมูล-(Important-Characteristics-of-Structured-Data)"
- มิติของข้อมูล (Dimensionality)
- Sparsity : สนใจเเค่จุดที่เเสดงหรือมีค่า ถ้าไม่มีค่าจะไม่สนใจ
- ความละเอียดของข้อมูลในการเเสดงผล (Resolution): รูปแบบขึ้นอยู่กับขนาดของข้อมูล
- การกระจาย (Distribution): ศูนย์กลางและการกระจายตัว Ex. mean, mode and median 

### Data Objects and Attribute Types
- Data Objects
- คุณลักษณะของข้อมูล (Attributes)
- ประเภทของคุณลักษณะของข้อมูล (Attribute Types) 
  - นามบัญญัติ (Nominal)
  - ข้อมูลที่ 2 ค่า (Bianry)
  - เรียงลำดับ (Ordinal)
- ประเภทคุณลักษณะของข้อมูลที่เป็นตัวเลข (Numeric Attribute Types)
  - เป็นข้อมูลเชิงปริมาณ (Quantity): จำนวนเต็มเเละจำนวนเต็ม
  - ข้อมูลระดับอันตภาคชั้น (Interval):ข้อมูลไม่ใช่ 0 เเท้, ลำดับข้อมูลมีค่า, ระยะห่างระหว่างค่าเท่ากัน Ex.อุณหภูมิในหน่วย C˚or F˚ ในแต่ล่ะวัน
  - ข้อมูลระดับอัตราส่วน (Ratio): ข้อมูลที่เป็น 0 เเท้ Ex.อุณหภูมิในหน่วยเคลวิน ความยาว นับ ปริมาณเงิน 
- Discrete vs. Continuous Attributes 
  - ข้อมูลที่มีลักษณะไม่ต่อเนื่อง (Discrete Attribute): มีเพียงชุดค่าจำกัดหรืออนันต์ที่นับได้เท่านั้น บางครั้ง แสดงเป็นตัวแปรจำนวนเต็ม Ex. รหัสไปรษณีย์ อาชีพ หรือชุดคำในชุดเอกสาร
  - ข้อมูลที่มีลักษณะต่อเนื่อง (Continuous Attribute): มีตัวเลขจริงเป็นค่าแอตทริบิวต์ ในทางปฏิบัติ ค่าจริงสามารถวัดและแสดงโดยใช้ตัวเลขจำนวนจำกัดเท่านั้น คุณลักษณะต่อเนื่องมักจะแสดงเป็นตัวแปรที่มีค่าเป็นทศนิยม Ex. อุณหภูมิ ส่วนสูง หรือน้ำหนัก

### Measuring Data Similarity and Dissimilarity
"การวัดความเหมือนและความแตกต่างของข้อมูล (Measuring Data Similarity and Dissimilarity)"

- Similarity, Dissimilarity, and Proximity
  - การวัดความเหมือนหรือฟังก์ชันความคล้ายคลึงกัน (Similarity measure or similarity function) : เป็นฟังก์ชันที่หาความคล้ายคลึงกันระหว่างสองอ็อบเจ็กต์วัดว่าออบเจ็กต์ข้อมูลสองรายการเหมือนกันแค่ไหน? ยิ่งค่าสูงเท่าไรก็ยิ่งเหมือนกันมากมักจะอยู่ในช่วง 0 ถึง 1 ; 0: ไม่มีความคล้ายคลึงกัน, 1: คล้ายกันโดยสิ้นเชิง
  - การวัดความแตกต่างหรือระยะทาง (Dissimilarity or distance measure) : การวัดเชิงตัวเลขว่าอ็อบเจ็กต์ข้อมูลสองรายการแตกต่างกันมากแค่ไหน? มีความผกผันกับความคล้ายคลึงกัน ค่ายิ่งต่ำยิ่งเหมือนกันมาก ความแตกต่างขั้นต่ำมักจะเป็น 0 (เช่น คล้ายกันทั้งหมด) ค่าจะอยู่ในช่วง ช่วง [0, 1] หรือ [0, ∞) ขึ้นอยู่กับคำจำกัดความ
  - การวัดความใกล้ชิด (Proximity):มักจะหมายถึงความเหมือนหรือความแตกต่าง

- เมทริกซ์ข้อมูลและเมทริกซ์ความแตกต่าง (Data Matrix and Dissimilarity Matrix)
  - เมทริกซ์ข้อมูล : เมทริกซ์ข้อมูลของ n จุดข้อมูลที่มีมิติ l ตามด้านล่าง
    <br /><p align="left"><a><img src="img/Chapter2_9.jpg" alt="Logo" width="600" ></a> </p><br /> 
  - เมทริกซ์ความแตกต่าง (ระยะห่าง) : n จุดข้อมูล แต่บันทึกเฉพาะระยะทาง d(i, j) (โดยทั่วไปของเมตริก) l ตามด้านล่าง ฟังก์ชันระยะทางมักจะแตกต่างกันสำหรับตัวแปรจริง บูลีน หมวดหมู่ ลำดับ อัตราส่วน และเวกเตอร์ 
    <br /><p align="left"><a><img src="img/Chapter2_10.jpg" alt="Logo" width="600" ></a> </p><br /> 

- การกำหนดมาตรฐานข้อมูลตัวเลข (Standardizing Numeric Data)
  -  Z-score: 
        Z = (X - M) /SD, 
        X = raw score, 
        M = Mean, 
        SD = Std. Deviation
  -  วิธีอื่น: คำนวณค่าเบี่ยงเบนสัมบูรณ์เฉลี่ย 
  -  การใช้ค่าเบี่ยงเบนสัมบูรณ์เฉลี่ยจะมีประสิทธิภาพมากกว่าการใช้ค่าเบี่ยงเบนมาตรฐาน 

- ระยะทางบนข้อมูลตัวเลข: Minkowski Distance 
  - Minkowski Distance -> เป็นการวัดระยะทางยอดนิยม 
  <br /><p align="left"><a><img src="img/Chapter2_11.jpg" alt="Logo" width="600" ></a> </p><br /> 
  คุณสมบัติ 
    - d(i, j) > 0 if i ≠ j, and d(i, i) = 0 (แง่บวก )
    - d(i, j) = d(j, i) (สมมาตร )
    - d(i, j) <= d(i, k) + d(k, j) (อสมการสามเหลี่ยม ) ;ระยะทางที่ตรงตามคุณสมบัติเหล่านี้เป็นหน่วยเมตริก 
   หมายเหตุ: มีความต่างที่ไม่ใช่เมตริก เช่น ความแตกต่างของเซต 
  - กรณีพิเศษของ Minkowski Distance  (Special Cases)
    <br /><p align="left"><a><img src="img/Chapter2_12.jpg" alt="Logo" width="600" ></a> </p><br /> 
  - Example: Minkowski Distance ในกรณีพิเศษ 
    <br /><p align="left"><a><img src="img/Chapter2_13.jpg" alt="Logo" width="600" ></a> </p><br /> 
- การวัดความใกล้เคียง (Proximity Measure)
  - การวัดความใกล้เคียงสำหรับตัวแปรไบนารี (Binary Attributes)
    -Distance measure for symmetric binary variables : ความน่าจะเป็นที่จะเกิด 2 ค่าเท่าๆ กัน 
    -Distance measure for asymmetric binary variables : ความน่าจะเป็นที่จะเกิด 2 ค่าไม่เท่ากัน 
    -Example:
     <br /><p align="left"><a><img src="img/Chapter2_14.jpg" alt="Logo" width="600" ></a> </p><br /> 
  - การวัดความใกล้เคียงสำหรับตัวแปรหมวดหมู่ (Categorical Attributes/nominal attributes)
    Method 1: Simple matching, m: # of matches, p: total # of variables
    <br /><p align="left"><a><img src="img/Chapter2_15.jpg" alt="Logo" width="600" ></a> </p><br /> 
    Method 2: ใช้แอตทริบิวต์ไบนารีจำนวนมาก, การสร้างแอตทริบิวต์ไบนารีใหม่สำหรับแต่ละหมวดหมู่ M  
  - การวัดความใกล้เคียงสำหรับตัวแปรลำดับ  (Ordinal Variables)
    > ตัวแปรลำดับอาจเป็นแบบไม่ต่อเนื่องหรือต่อเนื่องก็ได้, ลำดับมีความสำคัญ เช่น ยศ (เช่น น้องใหม่ รุ่นพี่ รุ่นน้อง รุ่นพี่)
   - สามารถคำนวณหาได้เหมือน interval-scaled:
   1.แทนที่ค่าตัวแปรลำดับตามอันดับ
   2.มปช่วงของตัวแปรแต่ละตัวลงบน [0, 1] โดยแทนที่อ็อบเจ็กต์ i-th ในตัวแปร f-th โดย สมการตามด้านล่าง
   ตัวอย่าง: น้องใหม่: 0; ปีที่สอง: 1/3; จูเนียร์: 2/3; รุ่นพี่ 1 จากนั้น ระยะทาง: d(น้องใหม่ รุ่นพี่) = 1, d(รุ่นน้อง รุ่นพี่) = 1/3 คำนวณความแตกต่างโดยใช้วิธีการสำหรับตัวแปรสเกลตาม interval-scaled

