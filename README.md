#
```
[1]標準輸入(stdin)與標準輸出(stdout)
   python輸入:input(), raw_input()
   python輸出: print()
   python格式化輸出技術
[2]
```
```
進階學習主題:
[10]讀取檔案與輸出到檔案
[20]資料庫讀取與輸出
```
# 基礎輸入與輸出(Basic Input and Output)

## 基本輸入:讀取使用者的輸入
```
使用input時，會從標準輸入(stdin)中讀取輸入資料
這些資料是string字串型態{重要}
stdin==Standard Input
```
```
# -*- coding: utf-8 -*-
x = input('Enter your name:')
print('Hello, ' + x)

a = input("請輸入：")
a

###  使用Python內建的type()函數顯示資料型態

type(a)
```

### 程式錯誤與更正
```
小明明正在學習python程式
老師出了一題
要輸入一個整數分數
然後加30後
輸出最後答案
底下是小明明的python程式
請指出底下的錯誤並更正
```
#### 小明明的python程式
```
a = input("請輸入：")
a
```
```
b=a+1
b
```
```
TypeError                                 Traceback (most recent call last)
<ipython-input-15-1bf84b7b9877> in <module>()
----> 1 b=a+1
      2 b

TypeError: must be str, not int
```
```
TypeError :資料型態(data type)錯誤
```
#### 更正的 小明明python程式
```
如何讀取使用者輸入的整數===>使用eval()函數
```
```
a = eval(input("請輸入："))
a

b=a+1
b
```
#### 超級重要:一次輸入多（兩）個資料
```
a,b = eval(input("請輸入兩個數位："))
a,b
```
### 高階技巧:[初學可略過]
```
x, y, z = [int(x) for x in input("Enter three value: ").split()] 
print("First Number is: ", x) 
print("Second Number is: ", y) 
print("Third Number is: ", z) 
print()

x, y, z = [int(x) for x in input("Enter three value: ").split(",")] 
print("First Number is: ", x) 
print("Second Number is: ", y) 
print("Third Number is: ", z) 
print()

a, b = input("Enter a two value: ").split() 
print("First number is {} and second number is {}".format(a, b)) 
print()
```
