# Rubyの配列との違い
- Javaの配列は、格納する要素の数を最初に決める必要があり、かつ後で要素数を変更することができない
- 要素を増やす場合は、サイズの大きな配列を新たに作成して元データをコピーするか、ArrayListというリストの一種を使用

# 配列の使い方を理解しよう
配列の使用手順  
1.配列の宣言を行う  
  - int型の整数を格納する配列の宣言はint[] scores;と記述
2.配列の要素を作成し、配列に代入する
  - scores = new int[3];
3.配列の要素に値を代入する
  - scores[0] = 1;
 
# 配列のさまざまな記述方法を理解しよう
① 配列の宣言と同時に、要素の作成も行う方法  
`int[] scores;`  
`scores = new int[3];`  
別の記述方法  
`int[] scores = new int[3];`  

② 配列の宣言時に型推論を使用する方法  
`var scores = new int[3];`  

③ 配列の宣言から値の代入まで全て同時に行う方法  
`int[] scores = {1, 5, 10};`  

# リストを理解しよう
特徴
- 要素を順序づけて管理する
- 要素を事後的に追加したり削除できる

種類
- ArrayList
- LinkedList

# ArrayList
- ArrayListは「可変長配列」を使用するための仕組み
- 可変長配列とは、文字通り長さ（要素数）を変更できる配列のこと

# ArrayListの使い方を理解しよう
1.ライブラリをインポートする
`import java.util.ArrayList;`
2.ArrayListの宣言を行う
`ArrayList<データ型> scores = new ArrayList<データ型>();`
3.ArrayListに値を代入する
`scores.add(1);`
4.ArrayListから要素を取り出す
`scores.get(0)`
