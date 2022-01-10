# コミットメッセージのテンプレート
commit.template  
システム上のファイルへのパスをここに設定すると、Git はそのファイルをコミット時のデフォルトメッセージとして使います。   
たとえば、次のようなテンプレートファイルを作って ~/.gitmessage.txt においたとしましょう。  

.gitmessage.txt
```
subject line

what happened
```
[ticket: X]
git commit のときにエディタに表示されるデフォルトメッセージをこれにするには、`commit.template` の設定を変更します。
```
$ git config --global commit.template ~/.gitmessage.txt
$ git commit
```

