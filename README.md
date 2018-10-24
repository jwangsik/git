# git 명령어

## git clone 
>origin 에 있는 repository 를 로컬로 가져오는 명령어. 

## git init 
>git 초기화  git clone 을 하게 되면 자동 수행 됨. 

## git add 
>작업내용을 등록하는 명령어

## git status 
>변경되고 commit 되지 않은 파일 목록을 보여 줌. 

## git commit 
>변경 내용 or 신규 추가 파일이 master 에 추가 됨. 
    

## git log 
>master 에 변경된 내용이 log 됨. 
            
## git push 
>master 의 수정 사항이 GitHub 의 origin repository 에 등록. 

## git branch 
>로컬의 branch 목록을 표시. 초기에는 master 만 표기됨.
    
## git checkout -b "브렌치 명"
> branch 생성. 
## git checkout "브렌치 명" 
>해당 branch 를 활성화 . 
 

## git reset 
>이전 단계로 되돌리는 방법. 로그를 확인해서 commit 된 상태의 키값을 확인 한다. 
     

## git 불필요한 revision 을 뭉개 없애기 
>git rebase -i HEAD~2 : 현재 branch 의 2개의 변경내용이 Editor 에 표시됨. 

