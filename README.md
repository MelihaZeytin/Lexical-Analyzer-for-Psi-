## Lexical rules for the programming language Psi++ are as follows:


1- Identifiers: 
- Maximum identifier size is 20 characters. If you use an identifier larger than that, the lexical analyzer issues an error message. 
-  Psi++ language is not case sensitive and all the identifier names are standardized as upper case. 
- Identifiers start with an alphabetic character (a letter) and are composed of one or more letters,digits or_ (underscore)

2- Integer constants
- Maximum integer size is 10 digits. If you use an integer value longer than that, the lexical analyzer issues an error message.
- Negative values are not supported.
-	Example Token: IntConst(1290)

3- Operators
-	Valid operators of the language are +,-,*,/,++,--,:=

4- Brackets
- LeftPar: (       			RightPar: )
- LeftSquareBracket: [		RightSquareBracket: ]
- LeftCurlyBracket:  {		RightCurlyBracket:  }

5- String constants
- String constants of Psi++ are delimited by double quotes (ASCII code 34)as in “this is a string”
- String constants have unlimited size
- String constants cannot contain the double quote character. when you reach one, the string terminates.
- If a string constant cannot terminate before the file end, there should be a lexical error issued.

6- Keywords:
- Keywords are: break,case,char,const,continue,do,else,enum,float,for,goto,if,int,
long,record,return,static,while
- Psi++ language is not case sensitive and all the keywords are standardized as lower case. You can write the same word as “while” OR “While” OR “WHILE” and they all generate the 


7- End of line:  ;
- Example Token: EndOfLine
8- Comments: Anything between (* and *) is a comment.
- If a comment cannot terminate before the file end, there should be a lexical error issued.
- Comments are just like blank space and they provide no tokens.

Project Defn: The Program should accept a source file called code.psi and produce a text file named as code.lex that contains all the tokens of the code.lex listed one after the other.


--------------------------------

## Dosya girdisi

![image](https://user-images.githubusercontent.com/109876399/193450760-72f5a7a6-446a-4573-82e4-1df32f3390a5.png)

## Dosya çıktısı

![image](https://user-images.githubusercontent.com/109876399/193450802-bf0bd308-d825-4495-a2f5-06177ac26ce2.png)
 

## 1.ERROR mesajı  

Girdilerde en sondaki comment kapatılmadığı için konsolda error mesajı verilmiştir ve programdan çıkılmıştır.

![image](https://user-images.githubusercontent.com/109876399/193450830-f5cfa5c5-9857-4622-a0b8-461e151445a7.png)

---------------------------------

## 2. girdi

![image](https://user-images.githubusercontent.com/109876399/193678109-672def50-bbc3-46bd-a7ca-347d1c7e19b4.png)

## 2. çıktı

![image](https://user-images.githubusercontent.com/109876399/193678194-8dce3dac-636e-4f69-8f52-f7a9dfd691a7.png)

## 2. ERROR mesajı

Girdilerde string ifadenin 2. Tırnağı kapatılmamıştır. Dolayısıyla program o noktaya kadar olan tokenları yazıp hata mesajı verip kapanmıştır.

![image](https://user-images.githubusercontent.com/109876399/193678344-1dd4abc7-3c06-4f0d-abb2-3d5c2d2a0bc7.png)

------------------------------------

## 3.girdi

![image](https://user-images.githubusercontent.com/109876399/193678448-5d7cca64-553e-404b-bb91-112833bd53c3.png)

## 3. çıktı

![image](https://user-images.githubusercontent.com/109876399/193678525-e060b238-a96b-49b1-a0fa-96d66def0dd4.png)

## 3. Ekstra ERROR mesajları

10 basamaktan daha uzun bir integer girildiği için ve 20 karakterden daha uzun bir identifier girildiği için hata mesajı verilmiş ve bu tokenlar çıktıya eklenmeyerek tokenlar oluşturulmaya devam edilmiştir.

![image](https://user-images.githubusercontent.com/109876399/193678658-de0da58f-12dd-4986-99c5-e07ea1d5b20f.png)
