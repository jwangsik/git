# git 명령어

git clone : origin 에 있는 repository 를 로컬로 가져오는 명령어.  
git init : git 초기화 git clone 을 하게 되면 자동 수행 됨. 
git add : 작업내용을 반영하는 작업. 
git status : 변경되고 commit 되지 않은 파일 목록을 보여 줌. 
git commit : 변경 내용 or 신규 추가 파일이 master 에 추가 됨. 
     --amend 옵션 : 직전에 commit 메시지를 수정. 
     -am 옵션 : add 와 commit 을 동시 진행. 

git log : master 에 변경된 내용이 log 됨. 
            --graph 옵션 : 시각적으로 확인. 
git push : master 의 수정 사항이 GitHub 의 origin repository 에 등록. 

git branch : 로컬의 branch 목록을 표시. 초기에는 *master 만 표기됨.
    * 은 현재 활성화 된 branch. 
     $ git branch -a     라고 하면 origin 의 목록까지 표시됨. 
git checkout -b "브렌치 명" : branch 생성. 
git checkout "브렌치 명" : 해당 branch 를 활성화 . 
git merge : 
      (1) 다시 master 로 가서, 
      (2) git merge --no-ff "브렌치명"        
merge 시에 충돌이 발생하면 : "fix conflicts and then commit the result" 라는 문구가 나옴. 
해당 파일을 열면 >>>>>> 이나 ====== 또는 <<<<<< 등으로 문제 부분이 나옴. 적절히 수정 후 다시 add 와 commit 을 진행 함. 

git reset : 이전 단계로 되돌리는 방법. 로그를 확인해서 commit 된 상태의 키값을 확인 한다. 
      ex) 7f3b80aab6e84768xxxxxx 등으로 시작되는 값. 
    $ git reset --hard "commit 된 키값" 

git 불필요한 revision 을 뭉개 없애기 : 
git rebase -i HEAD~2 : 현재 branch 의 2개의 변경내용이 Editor 에 표시됨. 
[출처] Git 명령어 정리|작성자 힌구름

