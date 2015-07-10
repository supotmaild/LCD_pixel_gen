# LCD_pixel_gen
LCD pixel font generator to write lcd_font.py that can import to your project 
- เน้นเรื่อง font ภาษาไทย สำหรับนำไปใช้ใน OpenCV หรือโปรแกรมที่ยังไม่สามารถใช้ True Type Font ได้โดยสะดวก
- ข้อมูลจะถูก save ไว้ที่ lcd_font.py 
- เรียกใช้งานโดย import lcd_font ในโปรแกรมของท่าน
- ตั้งค่าตัวแปรเช่น font_data = lcd_font.font()
- ตัวแปรของท่านจะอยู่ในรูป array ของรหัส ascii windows-874 มี 256อะเรย์
- ใช้งานโดย font.data[161][0] 161 คือ ก ไก่ [0] คือแนวตั้งแรกของ byte ที่ดอท pixel ได้ แปดหน่วย pixel บรรทัด
- วิธี byte แนวตั้งนำมาจากการ plot ของจอแบบ LCD ขาวดำทั่วไป ที่ใช้ในอิเลกทรอนิกส์ขนาดเล็ก
