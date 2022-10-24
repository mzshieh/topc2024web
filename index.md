## Latest News

### 2022/10/24

#### 重判報告 Rejudge report 

+ 因賽中 11:30 之後有感受到裁判機有些時候會卡住。經賽後針對超時的提交再次檢查，下表的 submission 均變成 `Correct` 。我們對受到不幸事故影響的隊伍感到抱歉。
+ After 11:30, we feel that some judgehosts were not responding. We have rechecked all `Time-Limit` results, and the following submissions should be correct. We apologize to the teams affected by this unfortunate accident.

|ID   |time |team        |problem|
|-----|-----|------------|-------|
|s2599|11:37|SplayTreap  |H      |
|s2617|11:39|felixtration|B      |
|s2693|11:45|Auto_temp   |H      |
|s2717|11:46|Auto_temp   |H      |
|s2726|11:47|NYCU_2434   |G      |
|s2789|11:52|NCUmix      |H      |
|s2801|11:52|CYFNZ       |B      |
|s2808|11:52|S@OAO!      |G      |
|s2864|11:55|S@OAO!      |G      |
|s2885|11:56|CYFNZ       |B      |

#### 裁判系統報告 Judge System Report

本次使用 DOMjudge 8.1.0 ，在正賽體驗到一些先前沒有的問題，以下條列並說明主辦處置。
+ 開賽後設定 Problem B 採用的 compare script 掛上 case_sensitive 的 argument ，想要再調整回 case insentitive 卻發現不能清空造成錯誤。default compare 吃到不存在的參數會 judge error，造成所有採用 default compare 的題目狀態切換成 not allow judge，在競賽初期造成影響，主辦單位只能盡速排除，無法提供補償。
+ 偶而會發生 judgehost 結果無法傳回或是卡死，因此賽中手動 rejudge 部份無傳回的 submssion ，事後 rechecking 所有 time-limit。僅更正因 judgehost 異常導致 time-limit 的測試結果。
+ 賽中發生數次 DB 大量存取導致系統卡頓或是 50x 系列錯誤，當下已盡量調整，不做補償。
+ 因 DOMjudge 內建 python3 執行環境改為 pypy (3.6.9)，非事前公佈的環境 3.8.10 or later，因而影響 Problem H 的標程執行效率與時限設定。此事命題階段、測試階段、正賽中均無人回報，公平性雖略受影響，但缺乏合適救濟手段，不予調整。

We used DOMjudge 8.1.0 and experienced some issues never happened before. We list the issues as follows.
+ During the contest, we added a case_sensitive flag to Problem B and soon found that we were unable to remove the flag without crashing the default compare script. Once the compare script crashes, all problems using that script would not allow judge. We tried our best to resolve the issue, and there is no compensation.
+ Some judgehosts sometimes could not report the judge results or just stucked. We manually rejudged those unresponsive submissions during the contest. Also, we have performed a rechecking on all `time-limit` submission. We have fixed all results related to this issue.
+ DOMjudge made several massive requests to the DB system and resulted in slowness or 50x errors. We have tried our best to resolve this issue during the contest. There is no compensation.  
+ The built-in python3 run script has been changed to use pypy 3.6.9, which is not Python 3.8.10 or later. It impacts the efficiency of Problem H's sample solution and Problem H's time limit settings. However, there was no one reporting this issue in the problem developing stage, the practice session, and the contest. We believe that the impact is minor, and it is hard to find a remedy. There is no compensation.

### 2022/10/22

+ [Problem archive](https://drive.google.com/file/d/11o2tOppq4_3jtGoEY4ZATHz1ysVmnbt7/view?usp=sharing)

### 2022/10/21

+ 因近期 COVID-19 疫情造成許多選手因病隔離，本次競賽開放異地參賽，
使用額外電腦登入裁判系統讀取題本、計分板、提問，透過通訊軟體、
電子白板 (如 Discord、Google meet、Google Jamboard 等) 與隊友溝通。
但仍禁止同時使用多台電腦同時撰寫程式碼及聯繫隊友之外的人。<br>
如無法全隊在教練所指定的地點參賽，
賽程中需對所有電腦之桌面進行錄影並錄下通訊程式的語音，
必要時提供給主辦單位檢視。如屆時無法提供錄影錄音，將被取消資格。
+ Since many contestants got COVID-19 and are in home isolation, 
we decided to allow teams to compete in separate spaces.
A team may use extra computers to access the judge system for 
problem statements, checking the scoreboard, and clarifications. 
But, simultaneously programming on multiple computers is still prohibited. 
Contestants may communicate with their teammates via communication software 
and digital whiteboards like Discord, Google Meet, and Google Jamboard. 
However, communicating with any person other than teammates is still prohibited. <br>
If your team cannot compete in the same place designated by your coach, 
then you have to record all screens of computers used and the communication 
with teammates during the contest. In addition, you must record the video 
with voice. We might ask you to provide the video clips for review when 
necessary. If you cannot provide the demand video, it may result in 
immediate disqualification. 

+ 錄影軟體可使用 [OBS Studio](https://obsproject.com/) 或是類似功能之軟體。
+ You may use [OBS Studio](https://obsproject.com/) or similar software 
to record the video.

### 2022/10/20
+ 已寄發帳號密碼等資訊給教練與參賽者，如未收到，請與我們聯繫，電子郵件信箱：mzshieh@nycu.edu.tw
+ We have delivered the contest information to coaches and contestants. If you did not receive the contest information, please contact us via E-mail: mzshieh@nycu.edu.tw

### 2022/10/16
+ 因 ICPC 官網系統障礙，報名延長至 2022 年 10 月 17 日。
+ The registration deadline has been extened to October 17, 2022. We will deliver team account information by October 20, 2022.

## Overview

1. **日期 Date** <br>
   2022 年 10 月 22 日 星期六 <br>
   Saturday, October 22, 2022
2. **地點 Place** <br>
   線上
   Online
3. **競賽時間 Contest Time** <br>
   早上九點至十二點 (三小時) <br>
   From 9:00 AM to 12:00 Noon (3 hours)
4. **題組 Problem Set** <br>
   總題數至少七題，所有題目均為英文，三分之一可由 Python 3 解出。
   賽後將提供中文題解資料。<br>
   There will be at least 7 problems to be solved. 
   The description of each problem will be available in English. 
   At least one third of them are solvable in Python 3. 
   For each problem, we will provide solution sketches in Traditional Chinese.
5. **報名 Registration** <br>
   請使用 ICPC 官方網頁註冊：<br>
   [https://icpc.global/regionals/finder/Taiwan-Online-2022](https://icpc.global/regionals/finder/Taiwan-Online-2022)
   <br>
   Please visit the official website of the ICPC:<br>
   [https://icpc.global/regionals/finder/Taiwan-Online-2022](https://icpc.global/regionals/finder/Taiwan-Online-2022)
6. **報名期限 Registration Deadline**<br>
   2022 年 10 月 16 日 星期日
   Sunday, October 16, 2022

## Eligibility

+ **基本資格規範 Basic Eligibility Rules** <br>
  請參照 ICPC [官方規範(連結)](https://icpc.global/regionals/rules) 中關於 Basic Eligibility Requirement 一節。<br>
  The eligibility rules are contained in the official regional 
  [rules](https://icpc.global/regionals/rules) on the ICPC website. See "Basic Eligibility Requirement" section. 

+ **隊伍組成 Team Composition** <br>
每隊由一名教練、三名參賽隊員、至多一名候補隊員組成。
教練為參賽學校之教職員，並獲學校授權，必須負責證實參賽隊員資格，
並負責與主辦方聯繫。參賽隊員與候補隊員需要滿足 ICPC 官方規範，
不可擔任教練。<br>
Each team must have a coach, three contestants and at most one reserved 
team member. The coach must be authorized to represent the school. 
The coach certifies the eligibilities of the contestants and 
is the official point-of-contact. All contestants and reserved team 
member must satisfy the ICPC official rules. None of them may serve as a coach.

## Ethics

參賽者應尊重對手，遵守規則，爭取個人、隊伍、學校的榮耀，維護社群的名譽。<br>
Contestants shall respect their opponents. Contestants shall abide the rules. 
Contestants shall compete for the honor of themselves, of their teams, 
and of their schools. Contestants shall not compromise the reputation of 
the society of competitive programming.

## Rules

賽前教練需上傳表格保證該隊伍遵照規則進行比賽。
如違反下列規則，將導致參賽者失去參賽資格。<br>
The coach has to submit a form to declare that the team abides by the rules 
during the contest. Contestants will be disqualified if they violate the 
following rules.

1. **不得使用機器可讀的資料 No machine-readable preparation**<br>
不得使用任何機器可讀的資料，如預先寫好存放於電腦中的程式碼。
但可以使用紙本資料，如教科書、字典、筆記以及列印好的紙本程式碼。<br>
No machine-readable materials (e.g., source codes, templates, etc.) 
are allowed. However, paper-based materials, such as textbooks, 
dictionaries, printed notes, etc., are allowed.
2. **僅與隊友接觸 Only contact teammates**<br>
在比賽過程中，參賽者只能與隊友討論。
競賽期間與教練或其他隊伍聯繫均屬違規行為。<br>
Contestants are allowed to contact only their teammates during the contest. 
Contestants shall not discuss with their coach and other teams.
3. **網路使用限制 Limited accesses**<br>
參賽者只能夠透過網路下載題目敘述、上傳解答程式碼、提問澄清疑點與查看計分板。
使用網路存取其他資訊均屬違規。<br>
Contestants shall access the internet only for downloading the problem 
description, submitting source codes, requesting problem clarification 
and checking the scoreboard. Any other type of internet access is prohibited.
4. **限用一台電腦 One computer**<br>
每個隊伍僅可使用一台電腦撰寫程式與上傳程式碼。
於競賽期間除使用印表機列印題目與程式碼以及透過額外的螢幕閱讀題目之外，
不得使用任何其他電子裝置。<br>
Each team shall not  use more than one computer to write programs 
during the contest. Contestant shall not use any other type of electronic 
devices, except extra monitors and printers.
5. **禁止惡意行為 No malicious actions**<br>
不得做出任何意圖妨礙比賽進行及影響比賽公平性的惡意行為。<br>
All malicious actions interfering the contest are prohibited.

## Scoring & Ranking

+ **計分與排名 Scoring & Ranking** <br>
隊伍以解題數量多者排名較前，解題數量相同時，以總消耗時間少者排名較前。
答對的題目的消耗時間計算方式為比賽開始至解出題目所消耗的分鐘數。
如解出前有答錯，每答錯一次需要另加 20 分鐘。
總消耗時間為所有答對題目的消耗時間加總。未答對的題目不計消耗時間。<br>
Teams are ranked according to the most problems solved. 
Teams who solve the same number of problems are ranked by least total time. 
The total time is the sum of the time consumed for each problem solved. 
The time consumed for a solved problem is the time elapsed from the beginning 
of the contest to the submittal of the accepted run plus 20 penalty minutes 
for every rejected run for that problem regardless of submittal time. 
There is no time consumed for a problem that is not solved.

+ **平手判定 Tie-Breaker**<br>
解題數與消耗時間均相同時，以先答對最後一題者獲勝。<br>
If multiple teams have the same number of problems solved and total time, 
then the winner goes to the team which first submitted their last accepted 
solution.

## Important Dates

+ **註冊截止日期：**<br>
2022 年 10 月 16 日<br>
End of registration: October 16, 2022
+ **寄發隊伍帳號密碼：**<br>
2022 年 10 月 20 日寄發給教練<br>
Team account information will be delivered to the coach by October 20, 2022.

+ **暫定測試時間：**<br>
2022 年 10 月 21 日 下午十二點三十分至十一點三十分 (台灣時間)<br>
Tentative practice session: 12:30-23:30 on October 21, 2022 (GMT+8)<br>

+ **競賽時間：**<br>
2022 年 10 月 22 日 上午九點至中午十二點 (台灣時間)<br>
Contest time: 9:00-12:00 on October 22, 2022 (GMT+8)

## Judge Environment

### Hardware
AWS t2.small instance

### OS
Ubuntu 20.04 or later

### Compiler/Runtime Environment/Interpreter
+ C: gcc 9.3.0 or later
+ C++: g++ 9.3.0 or later
+ Java: OpenJDK 14.0.2 (JRE & JDK) or later
+ Python: 3.8.10 or later
+ Kotlin: 1.5.21 on JRE 14.0.2 or later

### Flags (Tentative)
+ C: `gcc -x c -Wall -O2 -static -pipe -o "$DEST" "$@" -lm`
+ C++: `g++ -x c++ -Wall -std=c++17 -O2 -static -pipe -o "$DEST" "$@"`
+ Java: `java -Dfile.encoding=UTF-8 -XX:+UseSerialGC -Xss${MEMSTACK}k -Xms${MEMLIMITJAVA}k -Xmx${MEMLIMITJAVA}k '$MAINCLASS' "$@"`
+ Kotlin: `kotlin -Dfile.encoding=UTF-8 -J-XX:+UseSerialGC -J-Xss${MEMSTACK}k -J-Xms${MEMLIMITJAVA}k -J-Xmx${MEMLIMITJAVA}k '$MAINCLASS' "$@"`

### Lazy Evaluation

The result of a rejected submission is the first encountered error. We do **not** prioritize `timelimit`, `run-error`, `memory-limit`, `output-limit` and `no-output`. 

### Penalty

There is no penalty on compilation errors.

## Contact
Contest Managers: mzshieh@nycu.edu.tw
