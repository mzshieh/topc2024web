### Judging issues

本次競賽總共有兩次 rejudge 。
+ 9:04 檢視全場第一個 `TIME-LIMIT` s664，發現其執行時間並不足 1 秒，因此 rejudge ，結果是 `CORRECT`。經過初步研究後發現，可能是 judgehost 第一次啟動 Interpreter 時，有比較長的延遲，造成 Wall Time 超過寬限值 `1s|10%` ，確認後即刻修改寬限值為 `5s|10%` 。由於從提交到修正判定僅耗時 3 分鐘，除更正結果外，不再進一步調整成績。 
+ 12:12 重新檢視全場 Java 與 Python 的 `TIME-LIMIT` ，並調整寬限值為 `10s|10%` 並以單台 judgehost 進行 rejudge 。結果發現還是有 s951、s1801 從 `TIME-LIMIT` 變成 `WRONG-ANSWER`，以及 s1312 從 `TIME-LIMIT` 變成 `CORRECT` ，因提交 s1312 的隊伍在不久後便答對，其他兩個變成錯誤答案的提交也難以評估實際影響，因此除更正結果外，不再進一步調整成績。

未來使用 AWS 或是類似雲端平台建設裁判系統時，均建議調高寬限值到 `10s|10%` 。
