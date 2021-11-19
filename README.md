# DPDM2021
> SC 637 802 Data Pre-processing and Data Mining

## Yupaporn Wanna 645020061-2

![image](https://user-images.githubusercontent.com/54661241/125416505-19edf0cf-fca6-460f-81a3-af9d8edeccc6.png)

-------------------------------
# Table of contents

* ## บทที่ 1 introduction 
     
     ประกอบด้วย 
   
   *  ### เนื้อหา [link](https://github.com/Peckkie/DPDM2021/blob/main/Chapter1.md)
        * ทำไม Data Mining ถึงมีความสำคัญ
        * Knowledge Discovery Process
        * Data Mining in Business Intelligence
        * KDD Process: A View from ML and Statistics
        * Data Mining Functions 1 Pattern Discovery
        * Data Mining Functions 2 Classification and 3 Cluster Analysis
        * Data Mining Functions 4 Outlier Analysis
        
* ## บทที่ 2 การทำความเข้าใจข้อมูล (Getting to Know Your Data) 
     
    
     * ### เนื้อหา [link](https://github.com/Peckkie/DPDM2021/blob/main/Chapter2.md)
        * ประเภทของข้อมูล
        * ลักษณะสำคัญของโครงสร้างข้อมูล
        * ประเภทของข้อมูล Data Objects and Attribute Types
        * การวัดความเหมือนและความแตกต่างของข้อมูล (Measuring Data Similarity and Dissimilarity)
       
       ประกอบด้วย 3 เรื่องใหญ่ คือ
       
     * ### 1 Basic python [code](https://github.com/Peckkie/DPDM2021/blob/main/Data101(Chapter2).ipynb)
 
        * การตั้งชื่อตัวแปร Variable
            ข้อกำหนดในการตั้งชื่อตัวแปร
            1. ชื่อห้ามมีเว้นวรรค
            2. (พยายาม)ใช้ภาษาอังกฤษ
            3. ตัวเล็กกับตัวใหญ่ แตกต่างกัน (case sensitive)
            4. ห้ามใช้ตัวเลขเป็นตัวหน้า
        * Casting: int() float() str()
        * โครงสร้างข้อมุล Data structure
        * Loop
            :: การให้ทำงานที่มันซ้ำๆกัน หรือ ทำงานที่คล้ายๆ หลายๆ รอ

            - stetment:

            ```
            for ตัวแปรที่เราจะรับค่าจากลิสต์ in ลิสต์ที่ตเช้องการจะวนลูป :
                do samethong
                do another thong

            this is uotside the loob :: ไม่อยู่ในลูป for 
            ```
        * IF Condition statement 
            (if statement)
            ```python
            if เงื่อนไขที่เราจะตรวจสอบ (โดยอาศัยสัญลักษณ์เหล่านี้ ==, !=, <, >, <=, >=, in, not in, is_nall() ):
                ถ้าเงื่อนไขเป็นจริงทำ
            elif เงื่อนไขที่เราจะตรวจสอบ ต่อไปถ้าเงื่อนไขข้างบนไม่เป็นจริง:
                ถ้าเงื่อนไขเป็นจริงทำ
            elif เงื่อนไขที่เราจะตรวจสอบ ต่อไปถ้าเงื่อนไขข้างบนไม่เป็นจริง:
                ถ้าเงื่อนไขเป็นจริงทำ
            else: #ตรวจสอบเงื่อนไขตรวจสอบข้างบนเเล้วไม่เป็นจริง
                ทำงานที่ x
            ```
        * Function
        
            ส่วนประกอบ
            - input 
            - process(ไม่มีไม่ได้)
            - output
          
            ```python
            def ชื่อฟังก์ชั้น(input,...):
                งาน XXX
                งาน YYY
                return output
            ```
            f(x) = 2X ; 
            
            >f is the name of the function
           
            >x this tells you that x is the input

            >2x tells you what the function does (this function multplies the input values by 2)


     * ### 2 Data Visualization [code](https://github.com/Peckkie/DPDM2021/blob/main/Data101(Chapter2).ipynb)
 
        * 1) Eyesball the Data
        * 2) Statical deacriptive
        * 3) Visualization
          * Packege matplotlib
          * Boxplot
          * Scatter plot
          * Plot
          * Barchart
          * Histogram

     * ### 3 Distance and Numpy Array [code](https://github.com/Peckkie/DPDM2021/blob/main/Data103_(Chapter2_distance).ipynb)
 
        * Numpy Array
         
          * Create numpy array
          * คำสั่งสร้าง matrix เริ้มต้น zeros, ones
          * คำสั่งสร้าง matrix เริ้มต้นด้วย random
          * Indexing
        
        * Distance Matrix
          * Euclidean Distance $\sqrt{(x_1 - x_2)^2 - (y_1 - y_2)^2} $
          * Manhatton Distance ${|x_1 - x_2|+|y_1 - y_2|}$
          * Euclidean distance $\sqrt{(x_1 - x_2)^2 - (y_1 - y_2)^2} $ 

* ## บทที่ 3 การเตรียมข้อมูลข้อมูล (Data preprocessing) [code](https://github.com/Peckkie/DPDM2021/blob/main/Data_preprocessing_(Chapter_3).ipynb)
        
     * ประกอบด้วย 
        
        * Descriptive Statistics of Data
        * Missing value
        * Handling Missing Value1 (ลบค่า missing)
        * Handing Missing Value2 แทนด้วยค่าที่เหมาะสมหรือสร้าง class ใหม่
        * Handing Missing Value3 แทนด้วยค่ากลาง
        * Handing Missing Value4 แทนด้วยค่ากลางของกลุ่ม
        * การทำงานกับ datetime-timestamp
        * Smooth data by Binning
        * การต่อตาราง [PD] แนวแกน X
        * [PD] Group by
        * [PD] Sample record
        * [PD] Save File
        * [PD] การสร้างตาราง pandas 
* ## บทที่ 4 Mining Frequent patterns, Association and Correlation [code](https://github.com/Peckkie/DPDM2021/blob/main/Frequart_Patterm_Assosiation_Rules.ipynb)

* ## บทที่ 5 Classification

     ประกอบด้วย 3 เรื่องใหญ่ คือ

     * #### 1 Decision Tree Classification [code](https://github.com/Peckkie/DPDM2021/blob/main/Classification_(Decision_Tree).ipynb)
     
     * #### 2 Nearest Neighbors Classification [code](https://github.com/Peckkie/DPDM2021/blob/main/Classification(KNN_Evaluation).ipynb)
        
     * #### 3 Naive Bayes Classification [code](https://github.com/Peckkie/DPDM2021/blob/main/Classification_(Naive_Bayes).ipynb)

* ## บทที่ 6 Cluster Analysis Ex. K-means [code](https://github.com/Peckkie/DPDM2021/blob/main/Chaper_8_Clustering.ipynb)

-------------------------------
# Mini Project 

* ### 1 Code จัดการ dataset 
     
     * ##### 1) Code Download Data Source : COVID-19 Data by CSSE and worldometers [code](https://github.com/Peckkie/DPDM2021/blob/main/1_COVID_19_Data_Downloading_and_Cleansing_.ipynb)

     * ##### 2) Code Download Countries in the world by population (2021) [code](https://github.com/Peckkie/DPDM2021/blob/main/2_COVID_19_Data_Downloading_and_Cleansing.ipynb)
     
     * ##### 3) Code Visaulization data และตอบคำถาม 2 ข้อ [code](https://github.com/Peckkie/DPDM2021/blob/main/2_Merging_table_2_Data_Source.ipynb)

         * [1] เเสดงประเทศที่มีประชากรมากที่สุดเเละมีอัตราส่วนการเป็นโควิดเเล้วหายเท่าไหร่
         * [2] แสดงสัดส่วนคนที่ติดโควิดเเล้วเสียชัวิตมากที่สุด 5 ประเทศเเรกในทวีปยุโรปและเอเชีย

* ### 2 Code รวมของ project*** [code](https://github.com/Peckkie/DPDM2021/blob/main/Mini_Project_COVID19.ipynb)

* ### 3 PPT นำเสนอ [link](https://github.com/Peckkie/DPDM2021/blob/main/PPT_Mini_Project_COVID19.pdf)

-------------------------------
