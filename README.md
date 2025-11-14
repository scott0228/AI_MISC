# AI_MISC

▸ fd — 找檔案神器
比傳統 find 快 3～10 倍，還會自動忽略 .gitignore 裡的垃圾檔。
想找某個 config、某支 script？打 fd main.go 就能瞬間定位 🔥
▸ rg（ripgrep）— 搜文字的王者
比 grep 還快，能同時搜尋整個 repo。
我常拿它找「某函數被呼叫的位置」，秒出結果。
▸ ast-grep — 找「結構」不是文字
這個超神。可以搜尋程式碼語法樹（AST），不是單純比字。
例如想找「所有 var 宣告」或「老舊 API 呼叫」，ast-grep 一次就抓完。💡
▸ fzf — 結果太多？直接互動選！
配合前面那些工具一起用，像 fd | fzf。
超順流～可以模糊搜尋、上下鍵篩選，效率炸裂。⚡️
▸ jq — JSON 處理必備
像是資料界的魔法棒。可以把一整包 API 回傳的 JSON 自動轉換、篩選。
jq '.[] | select(.price > 0.5)' 這種指令幫我省下超多人工時間。
▸ yq — 處理 YAML / XML 的高手
用來改 Kubernetes、CI/CD 設定檔超順。
不再手動開檔改半天，直接一行 yq -e '.spec.template' deploy.yaml ✅