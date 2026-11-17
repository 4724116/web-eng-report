# 第8回 Webエンジニアリング演習 レポート
## 学籍番号
4724116
## コンポーネント構成
App
└── TodoList
    ├── TodoItem
    ├── TodoItem
    └── TodoItem
## `TodoItem`のProps型
import type { Todo } from "../types";

type TodoItemProps = {
    todo: Todo;
};

export function TodoItem({ todo }: TodoItemProps) {
    return (
        <li>
            <strong>{todo.title}</strong>
            <span> {todo.completed ? "(completed)" : "(uncompleted)"}</span>
            {todo.dueDate && (
                <span
                    style={{
                        color: todo.dueDate < new Date().toISOString().slice(0, 10) ? "red" : "black",
                    }}
                >
                    {" "}期限: {todo.dueDate}
                </span>
            )}
        </li>
    );
}
## 期限あり・なしの画面確認結果
1つ目のTODOに期限を設定した。
期限があるTODOだけ日付が表示されて、期限が過ぎている場合は赤文字で表示されていることを確認した。
期限が設定されていないTODOでは、期限が表示されていないことを確認した。
