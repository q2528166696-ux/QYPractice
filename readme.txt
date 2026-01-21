git init    -----git管理開始初始化
git status ----檢測當下文件狀態
git add （文件全名）管理此文件
git add .  -----管理剩餘文件
git commit -m"v1" ------提交版本
git reset --hard （版本號）----回滾
git reset --soft （版本號）-----回滾到add狀態
git reset --mix （版本號）-----回滾到紅色狀態
git reset HEAD----add之後回滾到紅
git log------查看版本
git reflog---查看所有版本
git checkout ------修改後紅回滾到綠

分支以及修復bug
git branch -------------------查看分支
git branch +（分支名）------建立新分支
git checkout + （分支名）---切換分支
git merge（master） + （分支名）---- 合并
可能產生衝突，手動修改
git branch -d + （分支名）----------刪除分支

工作流
git

github
git remote add origin + url---連接遠程倉庫
git push -u origin -------------向遠程推送代碼
git clone + url -----------------克隆遠程倉庫代碼
git checkout 分支  -------------切換分支