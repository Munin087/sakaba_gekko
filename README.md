# <div style="text-align: center;">某酒場 家具の位置データ</div>

# <div style="text-align: center;">目的</div>
<span style="font-size: 170%;">
家具の位置データをgitを使って操作履歴、家具位置のバックアップを管理する<br>
export履歴を家具の位置を変更するたびにgitに記録するのが目的
</span>

##  <div style="text-align: center;">使い方</div>
<span style="font-size: 170%;">
* 某酒場の操作 (家具に変更があった場合) <br>
  1. 画面左のメニューからSettingをクリック<br>
  <p><img src="README.md_parts/1_setting.png" width="70%" height="auto" alt="setting"></p>
  2. exportをクリックして文字列を表示させる<br>
  <p><img src="README.md_parts/2_export_click.png" width="70%" height="auto" alt="export_click"></p>
  3. exportの文字列をコピーする<br>
  <p><img src="README.md_parts/3_export_copy.png" width="70%" height="auto" alt="export_copy"></p>
<br>
* ここから文字列を貼りける操作<br>
1. ディレクトリ内のkagu_export_data.txtをエディタで開いて<br>
2. kagu_export_data.txtに書いてある文字列を削除<br>
3. 某所でコピーした文字列をに貼りけて保存<br>
おまけ この操作をターミナルで操作する場合は ディレクトリを移動して 次のコマンド打てok<br>
$ echo '某所でコピーした文字列' | > kagu_export_data.txt<br>
<br>
* ここからgitの操作<br>
1. cd ディレクトリ名<br>
2. git add .<br>
3. git commit -m $(LANG=C date +%F_%T_%Z) <br>
4. git push origin ブランチ名 <br>
<br>
## その他<br>
相談、質問、グループメンバー参加、などはIssueへ
</span></div>
