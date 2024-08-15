# google-calendar-spent-time-calculator
その日仕事に使った累積時間を案件ごとに計算するwebページ

# コンセプトの説明

たとえば、以下のように「test」というキーワードを共通して含む予定が3件登録されているとします。

この3件の予定の合計時間を算出するためのツールです。

<img width="293" alt="doc-cal-sample" src="https://github.com/user-attachments/assets/7c8a03cd-ec13-4f3a-904d-f93f0a21a56b">

# 画面の説明

テキストエリアに、改行区切りでキーワードを複数定義できます。「Store Keywords」ボタンを押すと、localStorageに記録し、リロードしても同じ値が保持されます。

「Authorize」ボタンを押して、Googleログインしてください。自動的にデフォルトのカレンダーで、当日の予定をキーワードで検索し、計算結果を画面に出力します。

<img width="366" alt="doc-ui" src="https://github.com/user-attachments/assets/1d57c218-1704-468c-82e7-eea600156c58">

今回の場合、「test」キーワードだけが検索結果にヒットしたため、testの合計、「02:45」が出力されている、というわけです。

# 使い方

そのままでは使えません。OAuth同意画面をご自身で構成し、OAuth Client IDを発行して、 `index.html` 内の該当箇所を書き換えてください。

