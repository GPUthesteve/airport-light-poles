![2022-4-22_15-3-29-795](https://user-images.githubusercontent.com/89721316/164645277-c2b43d7d-06bf-4682-8991-b2a9887570d3.jpg)
![2022-4-22_15-3-30-929](https://user-images.githubusercontent.com/89721316/164645285-de399302-145c-4853-885d-713c53bbee38.jpg)
# airport-light-poles//EN
im bored so i made this library, customizable library light to use w/ fsx/p3d airport projects.

Well, it contains BGL Library of "Lights" and effect itself (I use effect so there will be backward compatiblity to FSX).
You can place it using ADE as internal Library or use sth like visual scenery editor "Simdirector." for p3d or FSX's Object Placement Tool located in SDK..

About lighting effects, it's pretty simple to edit its color using this arrangement
while color start is day color and coler end is night color...
                          R    G   B  intensity(255 max)
             Color Start=255,  0,  0, 255
             Color End=  255,  0,  0, 255

Texturing...its simple...or complicated? some random UV were made there so...its just solid color. I'm not texture artist also so bear with it or edit it as you like
there's pole, guard and lamp cover. the color of light will correspond to lamp cover and effect.

Night texture? I let the simulator handle the pole...except the cover that I use the day texture for it...and it lits so its fine for now.

I mean, after you tweak some effect and compiled the model in MCX, please re-color the lamp cover to be the same so it would look nice as it lits and glow via effect.

//TH 
โปรเจคนี้ เกิดจากความว่างจัด และไม่อยากเล่นเกมอะไร(ชั่วครู่) ของผม ผมจึ่งนั่งขุดสนามต่างๆที่เคยทำ และก็พบว่า พวกไฟริมขอบเนี่ยผมยืมคนอื่นใช้ เลยมาลองมาทำเอง เก็บไว้ใช้งานอื่นก็ได้ 

ก็จะมีในส่วน Libary BGL ของตัวไฟ และก็พวก Effect ที่ทำให้สว่าง(ที่ผมใช้ Effect เพราะผมอยากให้เอากลับไปใช้ใน FSX ได้)
ผู้ใช้งานจะสามารถเอาไปลากลงสนามของท่าน ด้วยวิธีใดก็ได้ตามสะดวก อย่างเอาไปประกอบเป็น ADE Libary Object หรือลากวางสดๆ โดยใช้ Simdirector, Object Placement Tool สำหรับ p3d และ fsx ตามลำดับ

ในส่วนของสีไฟ จะปรับยังไงก็ได้ เป็น RGB 255-255-255   ในไฟล์ fx_light_(color).fx   ลองหาบรรทัดนี้แล้วแก้ดู ตามลำดับที่ให้ไว้                     
                          R    G   B  size(255 max)
             Color Start=255,  0,  0, 255
             Color End=  255,  0,  0, 255
และก็ Texture, ผมทำ UV ไม่เก่ง เลยต้องใช้สีระบายใส่เอา สีละพาท แบ่งเป็น ตัวดวงโคม(Lamp), ฐานรองไฟ(Guard), และขาตั้ง(Pole). อาจดูไม่สวย ลองปรับแต่งกันเองได้แล้วแต่สะดวก
Texture ตอนกลางคืน ผมปล่อยให้ตัวเสามันมืดไป เหลือแต่ตัวโคมทีใช้ Texture เดียวกันทั้งวันทั้งคืน(Emissive+Albedo)(ผมทำให้มันดูใสด้วยจะได้สวย และจะได้สว่างจาก Effect ที่ผมแปะไว้ข้างใน)
พูดถึงตัวโคม และสีไฟ หลังจากทำ Effect เสร็จ และไปปรับแต่งใน ModelConverterX แล้ว ไประบายสีตัวโคมให้เป็นสีเดียวกับไฟด้วย จะได้สวยๆ ผมแนะนำ
