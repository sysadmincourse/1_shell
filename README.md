# Bash 

## Дасгал 1

`dasgal_1` хавтаст дотроо нэгэн онцгой файлыг хайж олно.  
Уг дасгалыг хийснээр та Линукс систем дээр файл, болон хавтаснуудаар хэсэхэд хялбар мэт санагдах болно. Зарим файлууд нуугдсан хэлбэртэй байж болох бөгөөд нуугдсан файлыг харахдаа `ls -a` гэж харах боломжтой.
  
### Ашиглах командууд
 * `ls`
 * `cd`
 * `cat`

## Дасгал 2

`dasgal_2` хавтаст байгаа `input.txt` файлд bash гэдэг үг (том жижиг үсгийн ялгаа гаргахгүйгээр) хэдэн ширхэг бичигдсэнийг ол.  

### Ашиглах командууд
 * `grep`
 * `wc`
 
## Дасгал 3

10 удаа `hello` гэж хэвлэх скрипт бич.

### Ашиглах командууд
 * `echo`

## Дасгал 4

1, 2, 3, 4, 5, 6, 7, 8, 9, 10 гэх нэртэй 10 ширхэг хавтас үүсгээд, үүссэн хавтаснуудыг `ls` командаар харуулаад, бүх үүсгэсэн хавтаснуудаа эргээд устгах скрипт бич.  

Хавтсыг устгахад `rm` командыг `-r` тохиргоотой дууддаг.

### Ашиглах командууд
 * `mkdir`
 * `rm`
 

## Дасгал 5

Дараах команд нь банк бүрийн долларын ханшийн мэдээллийг татаж авч, `tmp.out` файлруу бичнэ.  
```shell
curl https://ikon.mn/xrates | grep -i -3 usd | grep ₮ > tmp.out
```

Тэгвэл уг командыг цаг тутам дуудаж, өмнөхөөсөө өөрчлөгдсөн байвал дохио өгөх скрипт бич. Дохио өгөхдөө дараах командыг ашиглана.
```shell
(speaker-test -t sine -f 1000) & pid=$! ; sleep 0.5s ; kill -9 $pid
```
Өмнөхөөсөө өөрчлөгдсөн эсэхийг шалгахдаа гаралт `diff -q` командаар шинэ файлыг хуучин файлтай нь харьцуулах бөгөөд `diff` командын exit status-аар нь харьцуулалт ялгаатай байсан эсэхийг мэдэж болно.

### Ашиглах командууд
 * `diff`
 * `sleep`
`

## Дасгал 6

`gcd.sh` гэдэг гэдэг скрипт бичих ба скриптийг дуудахдаа хоёр тоо дамжуулна (`./gcd.sh 12 18` г.м). Уг скрипт дамжуулсан хоёр тооны ХИЕХ-ийг гаралтаараа гаргана.


## Дасгал 7

Гараас $$N$$, болон $$N$$ ширхэг тоог хүснэгтэд уншиж аваад дараах сонголттой скрипт хэрэгжүүл.  
Хэрэв дараах тоонуудын аль нэгийг оруулахад харгалзах үйлдлүүдийг хийдэг байна.
  1. Шинэ тоог уншин хүснэгтийн төгсгөлд оруулна.
  2. Шинэ тоог уншин хүснэгтийн эхэнд оруулна. Ингэхдээ бүх тоонууд 1 байрлал хойшилж, дараагаар хамгийн эхэнд шинэ тоог оруулна.
  3. Оруулсан тоог хүснэгтээс хайж устгана.
  4. Хүснэгтийг хэвлэнэ.
.
