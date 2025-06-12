[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/w8H8oomW)
**<ins>Note</ins>: Students must update this `README.md` file to be an installation manual or a README file for their own CS403 projects.**

**รหัสโครงงาน:** 67-1_14_pps-r1

**ชื่อโครงงาน (ไทย):** การวิเคราะห์ความรู้สึกเชิงแง่มุมพร้อมการแสดงผลด้วยรหัสสี

**Project Title (Eng):** Aspect based Sentiment Analysis with Color Coded

**อาจารย์ที่ปรึกษาโครงงาน:** ผศ. ดร. ปกป้อง ส่องเมือง 

**ผู้จัดทำโครงงาน:** 
1. นางสาวสุชานาถ หันทยุง  6309681598  suchanat.han@dome.tu.ac.th
   
Manual / Instructions for your projects starts here !
## โปรแกรมที่ติดตั้ง
1. ติดตั้ง Python ในเครื่อง (สามารถใช้ Python เวอร์ชัน 3.12 หรือ 3.13) [ติดตั้ง Python](https://www.python.org/downloads/)
2. ติดตั้ง Git ในเครื่อง [ติดตั้ง Git](https://git-scm.com/downloads)

เมื่อติดตั้งแล้วสามารถตรวจสอบการติดตั้ง
เปิด Command Prompt พิมพ์
```bash
python --version
```
และตรวจสอบ Git
```bash
git --version
```
3. ทำการ clone git
```bash
git clone https://github.com/ComSciThammasatU/2567-2-cs403-final-submission-67-1_14_pps-r1.git
```
4. **ติดตั้งโมเดล**
ก่อนจะทำการใช้งานโปรแกรมได้ต้องมีการติดตั้งโมเดล 2 ตัวจากโฟลเดอร์ model ใน repository (เนื่องจากไฟล์มีขนาดใหญ่เกินกว่าจะอัพใน github จึงทำการอัพโหลดแยกไว้ที่ Google Drive)
   1) MLTC_model_state.bin
   2) Sentiment_model_state.bin

5. **ลงไลบรารีที่ต้องใช้**
สามารถติดตั้งได้ 2 วิธี
   5.1 เมื่อเปิดใช้งาน cmd สามารถติดตั้งจากไฟล์ requirment.txt ที่ได้จาก git clone ในโฟลเดอร์ src
```bash
pip install -r requirements.txt
```
   5.2 ใน cmd พิมพ์
```bash
pip install pandas transformers scikit-learn seqeval torch Flask
```

## เริ่มต้นใช้งานโปรแกรม
เปิดโฟลเดอร์ src ที่ได้มาจากการ git clone
1. นำโมเดล 2 โมเดลที่ดาวน์โหลดมา ไปใส่ไว่ในโฟลเดอร์ src ที่ได้จาก git clone ด้วย
   1) MLTC_model_state.bin
   2) Sentiment_model_state.bin
  
2. ในโฟลเดอร์ src พิมพ์ใน cmd
```bash
python project.py
```
3. รอโปรแกรมรันลิ้งก์ขึ้นมา จากนั้นเปิด browser (เช่น chrome, microsoft edge) แล้วพิมพ์
```bash
127.0.0.1:5000
```
4. พิมพ์ประโยคที่ต้องการทดสอบบนหน้าเว็บแล้วกด Analyze
