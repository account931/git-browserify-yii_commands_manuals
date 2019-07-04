# git_commands
#List of most used Git commands

=================================================================================================



//Upload to github -------------------------------------------

$ git remote add origin REMOTE_REPOSITORY_URL    ->select reposotory, i.e https://github.com/account931/git_test/

$  git remote set-url origin REMOTE_REPOSITORY_URL   -> change repository, if was set prev

$ git push origin master       -> upload to github

$ git clone https://github.com/account931/yii2_REST_and_Rbac_2019.git  -> clone Git repo to local hdd





//add all modified to tracked(before $git commit)---

git add .   -> add all new untracked(mostly used)

git add -u  -> add to commit all tracked

git commit  -> save changes to commit(after {git add .})



//Branches-------------

$ git branch   -> check branches lists ->list of all branches

$ git checkout master   -> switch to master branch

$ git checkout -b issue53    ->create and switch to new branch "issue53"



See all commits history---------------------------------

$git log

$ git reset --hard 1a410efbd13591db07496601ebc7a059dd55cfe9    ->restore some version


============= STOP tracking some files ===========

$ git update-index --assume-unchanged Credentials/php_api_credentials/api_credentials.php  -->stop tracking some file

$ git update-index --no-assume-unchanged <file>  --> to start tracking that file again
  
$ git ls-files -v|grep '^h   --> see list of all untracked

Or add to .gitignore  --> /folderName/

=========================================

git config core.autocrlf true  -> get rid off "LF will be replaced by CRLF"


https://ru.stackoverflow.com/questions/431520/%D0%9A%D0%B0%D0%BA-%D0%B2%D0%B5%D1%80%D0%BD%D1%83%D1%82%D1%8C%D1%81%D1%8F-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C%D1%81%D1%8F-%D0%BA-%D0%B1%D0%BE%D0%BB%D0%B5%D0%B5-%D1%80%D0%B0%D0%BD%D0%BD%D0%B5%D0%BC%D1%83-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D1%83
