# 第5回 Webエンジニアリング演習 レポート
## 学籍番号
4724116
## TODO配列のコード
const todos = [
  { id: 1, title: "型を復習する", completed: true },
  { id: 2, title: "配列を学ぶ", completed: false },
  { id: 3, title: "レポートを書く", completed: true },
];
## TODOを更新した条件
for (const todo of todos) {
    if (todo.completed === false) {
        todo.completed = true;
        console.log(`更新後: ${todo.title} [完了]`);
    }
## 完了件数の更新前後の実行結果
完了件数: 更新前 2件 -> 更新後 3件
