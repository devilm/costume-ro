อีกจุดที่ควรแยกคือ ตอนโปรแกรมทำงาน --headgear=1 จะเรียก ReqAccName(1) จาก accname_f.lub 
เพื่อหาชื่อไฟล์ sprite ที่ต้องโหลด ตาม logic ใน resolver.d 
ดังนั้น accessoryid.lub ใช้ดูความหมาย/เลข ID ส่วน accname_f.lub ใช้แปลง ID เป็นชื่อ resource สำหรับ render ครับ

ีunluac
headgear
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\accessoryid.lub" > "C:\Users\tanak\Downloads\accessoryid-decoded.lua"
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\accname_f.lub" > "C:\Users\tanak\Downloads\accname_f-decoded.lua"
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\accname.lub" > "C:\Users\tanak\Downloads\accname-decoded.lua"
garment
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\spriterobename.lub" > "C:\Users\tanak\Downloads\spriterobename-decoded.lua"
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\spriterobename_f.lub" > "C:\Users\tanak\Downloads\spriterobename_f-decoded.lua"
java -jar ""C:\Users\tanak\Downloads\data\unluac_2025_12_23.jar"" "C:\Users\tanak\Downloads\data\luafiles514\lua files\datainfo\spriterobeid.lub" > "C:\Users\tanak\Downloads\spriterobeid-decoded.lua"


enluac
luac -o "C:\Users\tanak\Downloads\accessoryid-new.lub" "C:\Users\tanak\Downloads\accessoryid-decoded.lua"