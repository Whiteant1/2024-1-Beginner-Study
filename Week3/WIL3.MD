# 3주차 Weekly-I-Learn
* * *
## commit 관련 명령어와 commit 의 작동 방식을 배웠다.
### git log
- commit 기록 확인
### commit id
- 40자 길이의 16진수로 되어있으며 중복되면 SHA-1해시 함수를 사용하여 구분
### HEAD
- 현재 작업 중인 위치를 가리킴 (pointer)
### commit --amend
- 마지막 commit 내용에 변경이 있을 때 사용
- git commit --amend -m "커밋 메시지"
- git commit --amend --no-edit  (커밋 메시지 수정X)
### reset
- commit id를 사용하여 커밋을 되돌림
- reset --soft: 커밋 취소 후 Staging Area로
- reset --mixed: 커밋 취소 후 Working Directory로
- reset --hard: 커밋 완전 삭제
### revert
- commit을 삭제하지 않고 이전 commit을 되돌린 commit을 새롭게 생성
- 이전 커밋을 되돌리므로 reset 보다 안전함