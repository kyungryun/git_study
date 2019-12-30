# Do It Git 책 공부 내용 정리

## Git 명령어

커밋 로그 확인
- git log
커밋에 관련된 파일 확인
- git log --stat

커밋 메시지 수정
- git commit --amend

수정한 파일 되돌리기
- git checkout -- file

스테이징 되돌리기
- git reset HEAD file

최신 커밋 되돌리기
- git reset HEAD^

**reset HEAD^ 명령어에 사용할 수 있는 옵션**
옵션  | 내용 
----- | ----- 
--soft HEAD^ | 최근 커밋을 하기 전 상태 
--mixed HEAD^ | 최근 커밋과 스테이징을 하기 전 **reset HEAD^ 디폴트 옵션**
--hard HEAD^ | 최근 커밋과 스테이징, 파일 수정을 하기 전

특정 커밋으로 되돌리기
- git reset 커밋 해시

커밋 삭제하지 않고 되돌리기
- git revert
