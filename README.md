Клонувати репозиторій
git clone --recursive https://github.com/den-vasyliev/gohttps
git fetch --all

Змінити гілку на вказану у повідомленні
git switch -c feature/metrics remotes/origin/feature/metrics

Перевірити лог комітів та знайти хеш коміту з фіксом
git log --> (d1ac709120)

Повернутися на головну гілку
git checkout main

Виконати cherry-pick для коміту з фіксом
git cherry-pick d1ac709120


Перевірити виправлений код 
nano main.go


Підтвердити зміни git log --oneline
9c4d78f (HEAD -> main) fix default port to 9000
aa85cde (origin/main, origin/HEAD) improved by GPT
ae8b3d1 add project description
94df9be add comments by ChatGPT
40ee074 init

