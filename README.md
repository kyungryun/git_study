# Do It Git 책 공부 내용 정리

## Git 명령어

커밋 로그 확인
- git log
    - 커밋에 관련된 파일 확인
      - git log --stat
    - 한 줄에 한 커밋씩 나타내기
      - git log --oneline
    - 각 브랜치의 커밋 내용 보기
      - git log --oneline --branches
      
- git log --stat

변경 사항 확인 하기
1. 작업 트리에 있는 파일과 스테이지에 있는 파일을 비교
2. 스테이지에 있는 파일과 저장소에 있는 최신 커밋을 비교
- git diff

커밋 메시지 수정
- git commit --amend

작업 트리에서 수정한 파일 되돌리기
- git checkout -- file

스테이징 되돌리기
- git reset HEAD file

최신 커밋 되돌리기
- git reset HEAD^

**reset HEAD^ 명령어에 사용할 수 있는 옵션**  

옵션  | 내용 
----- | ----- 
--soft HEAD^ | 최근 커밋을 하기 전 상태 
--mixed HEAD^ | 최근 커밋과 스테이징을 하기 전 **reset HEAD^ 기본 옵션**
--hard HEAD^ | 최근 커밋과 스테이징, 파일 수정을 하기 전


## checkout, reset HEAD, reset HEAD^ 비교

git checkout | git reset HEAD | git reset HEAD^
------------ | -------------- | ---------------
변경 사항 되돌리기 | 스테이징 취소 하기 | 커밋&스테이징 취소하기


특정 커밋으로 되돌리기
- git reset 커밋 해시

커밋 삭제하지 않고 되돌리기
- git revert

## Branch

현재 브랜치 확인
- git branch

새로운 브랜치 만들기
- git branch name

브랜치 이동
- git checkout name


