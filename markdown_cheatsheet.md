# マークダウン記法のチートシート

## 第２段落

### 第3段落

### 改行
いろはにほへと　ちりぬるを  
わかよたれそ　つねならむ  
半角2行を末尾に入れることで改行できる  

### 強調
**強調は２つのアスタリスクで囲む**  
__または２つのアンダースコアで囲む__  
*ひとつだけなら斜体になる*

### リスト
リストを示す場合は：
* アスタリスク(\*)
- またはハイフン(-)
+ またはプラス(+)

### 順序リスト
順序リストは  
1. 数字とピリオドで。
2. にい
3. さん

### 罫線
罫線は３つ以上の\* or - or +  
---  
*****  
++++++  

### リンク
角括弧[]で文言、丸括弧()でURLを囲むとリンクになる
- [参考](http://kojika17.com/2013/01/starting-markdown.html)
- [これまた参考](http://qiita.com/tbpgr/items/989c6badefff69377da7)

### 引用
行頭に>をつける
> お世話になります
>
> どうもです。
>
>> ふたつつければ
>>
>> 二重引用にできる
>

### code記法
バッククォートで文字列を囲む
`printf("hello, world");`

### 取り消し線
Githubだけで使用できるもよう。
~~こんなかんじで2つチルダで囲む~~

### 文法ハイライト
チルダのあとに言語名を記述
~~~python
def printHello():
    print("hello, markdown")
~~~

### 表
|header1|header2|
|:--|--:|
|なんか縦棒で囲む|詳しいことは分からん|

### omake
Atomエディタで、`[ctrl]+[shift]+m`
で、マークダウンをプレビュー表示できる。
