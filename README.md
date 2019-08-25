# git_commands
#List of most used Git commands

=================================================================================================



===================Upload to github========================

$ git remote add origin REMOTE_REPOSITORY_URL    ->select reposotory, i.e https://github.com/account931/git_test/

$  git remote set-url origin REMOTE_REPOSITORY_URL   -> change repository, if was set prev

$ git push origin master       -> upload to github

$ git clone https://github.com/account931/yii2_REST_and_Rbac_2019.git  -> clone Git repo to local hdd

$ git pull origin -> updates any changes from Git repo to local HDD project






===============add all modified to tracked(before $git commit)=================

git add .   -> add all new untracked(mostly used)

git add -u  -> add to commit all tracked

git commit  -> save changes to commit(after {git add .})



=========================Branches=====================

$ git branch   -> check branches lists ->list of all branches

$ git checkout master   -> switch to master branch

$ git checkout -b issue53    ->create and switch to new branch "issue53"


$ git checkout master  $git merge BRANCH_NAME  -> merge your new created branch to master branch(firstly you need to check-out to master)




=======================See all commits history, RESTORE/REVERT BACK to SOME COMMIT=====================================

$git log

$ git reset --hard 1a410efbd13591db07496601ebc7a059dd55cfe9    ->restore back some old version. Dangerous, it will erase any commits those were up to restoring point.


SAFER VARIANT-----

$ git reset --hard HEAD   -> To revert to a previous commit, ignoring any changes.

IF u want to revert to a commit that's older than the most recent commit, use next 4 lines of commands:

git reset 56e05fced   -> # Resets index to former commit; replace '56e05fced' with your commit code

git reset --soft HEAD@{1}  -> # Moves pointer back to previous HEAD

git commit -m "Revert to 56e05fced"

git reset --hard  ->  # Updates working copy to reflect the new commit

END SAFER VARIANT----




============= STOP tracking some files ===========

$ git update-index --assume-unchanged Credentials/php_api_credentials/api_credentials.php  -->stop tracking some file

$ git update-index --no-assume-unchanged <file>  --> to start tracking that file again
  
$ git ls-files -v|grep '^h   --> see list of all untracked

Or add to .gitignore  --> /folderName/

=========================================

git config core.autocrlf true  -> get rid off "LF will be replaced by CRLF"


https://ru.stackoverflow.com/questions/431520/%D0%9A%D0%B0%D0%BA-%D0%B2%D0%B5%D1%80%D0%BD%D1%83%D1%82%D1%8C%D1%81%D1%8F-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C%D1%81%D1%8F-%D0%BA-%D0%B1%D0%BE%D0%BB%D0%B5%D0%B5-%D1%80%D0%B0%D0%BD%D0%BD%D0%B5%D0%BC%D1%83-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D1%83
