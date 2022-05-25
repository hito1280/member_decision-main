# 使う前に
pip install -r requirements.txt
で必要なものをインストールしてください。

# 割り当て
## 予定表のダウンロード
鍵締めのスプレッドシートより
ファイル>ダウンロード>カンマ区切り方式
で予定表を.csv形式でダウンロードしてください。

### スプレッドシートについて
*制限*
* このプログラムでは鍵閉めの表とゴミ捨ての表の間の空の列で両者を区別しています。
* 鍵閉めの表に含まれる名前は必ずゴミ捨ての表にも含めるようにしてください。
* 上記制限を守れば人の追加、削除は可能です。

月に1回masterおよびmaster2はコピーされ、新しい月の予定表、配置になります。
休日は休日一覧より取得しています。（これも年に一度更新されます。）

研究室で実験禁止となっている日など、休日でないが当番を割り当てる必要がない場合には実験禁止など（空欄でなければなんでも構いません）と記入してください。

## 割り当ての実行
main.pyで実行できます。（これは乱数で決めるだけです。）
ダウンロードした予定表のパスをinput_pathに、割り当て後の配置とカレンダーファイルを保存したいフォルダをdir_outputに指定してください。

terminalより
python main.py
で実行してください。

csv形式の配置表とicalファイルがdir_outputに指定したフォルダに保存されます。
配置表をスプレッドシートにコピーし、icalファイルはメール等で共有してください。
当番決定後はシートに保護の設定をすることをお勧めします。

