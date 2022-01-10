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
---

# ==================== Emojis ====================
# 🎉  :tada: 初めてのコミット（Initial Commit）
# 🔖  :bookmark: バージョンタグ（Version Tag）
# ✨  :sparkles: 新機能（New Feature）
# 🐛  :bug: バグ修正（Bugfix）
# ♻️  :recycle: リファクタリング(Refactoring)
# 📚  :books: ドキュメント（Documentation）
# 🎨  :art: デザインUI/UX(Accessibility)
# 🐎  :horse: パフォーマンス（Performance）
# 🔧  :wrench: ツール（Tooling）
# 🚨  :rotating_light: テスト（Tests）
# 💩  :hankey: 非推奨追加（Deprecation）
# 🗑️  :wastebasket: 削除（Removal）
# 🚧  :construction: WIP(Work In Progress)


# ==================== Format ====================
# :emoji: Subject
#
# Commit body...
