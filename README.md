# Machine-4 "DeathNote 1: Vulnhub"
**1.** Эхлээд бид хохирогчийн машины IP хаягийг **netdiscover** ашиглан шалгах болно.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/44c57875-db81-43d3-adb3-af469537f9bd)

**2.** Дараа нь бид nmap ашиглан нээлттэй портуудыг олох хэрэгтэй.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/e16fbe10-1452-4163-9a88-7cef9c908580)

Энд бидэнд хоёр порт нээлттэй байна. **HTTP-д 80, SSH-д 22**.
**3.** Бид вэб хөтчөө ашиглан вэбсайтыг нээнэ. Бид 10.10.10.2 гэж бичнэ (Алдаа гарч ирвэл IP хаягийг /etc доторх хост файлд нэмнэ үү). Бид зөвлөмжийн товчлуурыг олдог. Үүн дээр дарцгаая.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/1b538dd7-30b1-4d59-825c-5516ab4dfb2c)

Энэ нь биднээс note.txt файлыг олохыг хүсч байна. Хуудасны эх кодыг үзэх замаар бид ямар нэг зүйлийг олж мэдэх боломжтой эсэхийг харцгаая.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/479cba2a-8e24-4784-812c-138ae3d9d4a5)

Бид **/wordpress/wp-content/uploads/2021/07** лавлахыг олдог

Үүнийг шалгаж үзье

![image](https://github.com/Bultuush/Machine-4/assets/129934501/23a911ba-5271-4891-af40-10670b478f58)

Хараач, бид **Notes.txt** файлыг аль хэдийн олсон! Мөн **user.txt** файл байна.
Тэдний агуулгыг харцгаая.
![image](https://github.com/Bultuush/Machine-4/assets/129934501/125cbcc5-849a-4fa3-98b4-67bf706998de)
![image](https://github.com/Bultuush/Machine-4/assets/129934501/fc1c3305-1c70-43a6-8add-e88b08b9a1da)

Хэрэглэгчийн нэрсийн жагсаалт шиг харагдаж байна. Бид үүнийг дараа нь нэвтрэх хуудас руу довтлоход ашиглаж болно

**4.** Хязгаарлагдмал сангуудын талаар дэлгэрэнгүй мэдээлэл байгаа эсэхийг мэдэхийн тулд **robots.txt**-г хайж байна.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/48d84f06-b4bc-4464-88aa-ef4794223fd5)

**Light’s Dad important.jpg** файлд зөвлөмж нэмсэн

Зурган дээрх өгөгдлийг буцаахын тулд бид **curl** ашигладаг.
![image](https://github.com/Bultuush/Machine-4/assets/129934501/b7f17910-3d8b-47e2-a785-5fa99c071814)

Энэ нь **user.txt**-г хэрэглэгчийн нэрэнд үгийн жагсаалт болгон ашиглаж, **notes.txt**-г нууц үгэнд ашиглаж болохыг баталж байна.
**5.** Зорилтот машин руу нэвтрэхийн тулд hydra-г ашиглах

![image](https://github.com/Bultuush/Machine-4/assets/129934501/83d1f11c-51b6-4b86-9ae3-9429ed4a5491)

Бид user-ийг олсон: **l** нууц үг: **death4me**.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/5fb0ab99-454c-40f3-93ce-3ca1cfcfe4ae)

Хэрэгтэй мэдээлэл олж чадах эсэхийг харахын тулд илүү гүнзгий судалцгаая.

**cat user.txt**

![image](https://github.com/Bultuush/Machine-4/assets/129934501/e59a387a-5b1f-41fd-b00d-aa79cbe8e65f)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/c5fd37c7-b36e-40ff-9312-b22731f82d77)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/c5feb4e6-8d9e-44aa-939f-4df98f079766)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/22a50cb4-7161-44b1-9335-6e1d0c26a3a7)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/e784f30c-c2cc-40f6-acdf-94dda30313d1)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/af610bdd-40ec-40cf-8642-2d3f636a12f7)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/bffffe5b-82f6-4d07-ae6a-98fd0c5e0a77)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/b9628316-d051-49a8-804b-6be25697c78e)

**/opt/L** дотроос 2 лавлах олдсон.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/77559926-15ee-42f5-b72b-a7f7fd32b05c)

**case.wav** файлаас хэш код олдсон бололтой, cyberchef ашиглана уу гэсэн зөвлөмж байна.

Hex код шиг харагдаж байна. Үүнийг задлахын тулд cyberchef-ийг ашиглацгаая.

![image](https://github.com/Bultuush/Machine-4/assets/129934501/811e8299-2c79-4d87-ad71-cdb5ccec9144)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/f484c5e9-094a-4ce3-8144-49840ade7652)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/dfb2e8b0-01ed-4201-a415-fad01624f6d1)

![image](https://github.com/Bultuush/Machine-4/assets/129934501/719c17c6-da8d-4ebc-a1f7-d28005f6c43e)
