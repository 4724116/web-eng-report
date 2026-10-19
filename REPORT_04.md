# 第4回 Webエンジニアリング演習 レポート
## 学籍番号
4724116
## `const`と`let`の宣言・再代入に使用したコード
const courseName = "Web Engineering";
let retryCount = 1;

courseName = "Other Course";
retryCount = 2;

console.log(`Course: ${courseName}`);
console.log(`Retry count: ${retryCount}`);
## VSCodeと`pnpm run check`に表示されたエラー番号・メッセージ
$ tsc --noEmit src/index.ts
src/index.ts:21:1 - error TS2588: Cannot assign to 'courseName' because it is a constant.

21 courseName = "Other Course";
   ~~~~~~~~~~


Found 1 error in src/index.ts:21

[ELIFECYCLE] Command failed with exit code 2.
## 修正後の実行結果と`const`・`let`の違いの説明
$ tsx src/index.ts
キーボード 4800 2 true
10560
商品名: キーボードを2個購入しました。合計金額は10560円です。
Course: Web Engineering
Retry count: 2
const は変数名への再代入を防ぐ
let は後から値を入れ替えられる
