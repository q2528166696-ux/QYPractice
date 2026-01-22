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

正常流程
在新電腦獲取代碼
1，克隆遠程代碼     git clone + url
2，切換分支            git checkout 分支

在公司新電腦進行開發
1，切換dev進行開發   git checkout dev
2，把master分支合并到dev   git merge master
3，修改代碼
4，提交代碼：git add . -----> git commit -m' ' -----> git push origin dev

回家繼續寫代碼
1，切換到dev分支進行開發  git checkout dev
2，拉代碼 	git pull origin dev
3，繼續寫代碼
4，提交代碼：git add .---->git commit -m' ' -----> git push origin dev

開發完畢要上綫
1，將dev分支合并到master，進行上綫		git checkout master---->git marge dev ----> git push origin master
2，把dev分支推到遠程	git checkout dev---->git merge master---->git push origin dev

if沒有推到github
回家之後繼續開發，推到github
用公司電腦 git pull origin dev，再繼續手動添加修改










