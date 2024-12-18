 HEAD
# 깃 명령어 정리 📘

 이 문서에서는 자주 사용하는 깃 명령어를 간단히 정리

| 명령어                   | 설명                                      | 이모지  |
|--------------------------|-------------------------------------------|---------|
| `git init`              | 새로운 깃 저장소를 초기화                 | 🚀      |
| `git status`            | 현재 작업 디렉토리 상태 확인              | 📋      |
| `git add .`             | 모든 변경 파일을 스테이징 영역에 추가     | 📥      |
| `git commit -m "메시지"` | 변경사항 커밋                             | ✅      |
| `git branch`            | 브랜치 목록 확인 및 생성                  | 🌿      |
| `git checkout 브랜치명` | 특정 브랜치로 이동                       | 🔀      |
| `git merge 브랜치명`    | 브랜치 병합                              | 🔗      |
| `git pull`              | 리모트 저장소에서 변경사항 가져오기       | ⬇️      |
| `git push`              | 로컬 변경사항을 리모트 저장소로 푸시      | ⬆️      |
| `git clone URL`         | 리모트 저장소 복제                       | 🛠️      |
| `git log`               | 커밋 로그 확인                           | 🕒      |
| `git blame 파일명`       | 파일에서 각 줄의 마지막 수정자 확인       | 🕵️      |

### 추가 설명
- **`git blame`** 🕵️  
  특정 파일의 각 줄에 대해 마지막으로 변경한 사람이 누구인지, 그리고 언제 수정되었는지를 확인

오늘의 실습 : 레포지토리 초기화해보기

원격저장소 가져오기
> git clone 레포지토리주소

내 로컬 저장소 git 환경 초기화
> git init

내 파일 변경사항 모두 저장
> git add .

변경사항을 이력에 남기기
> git commit -m "커밋메세지"
> 커밋 메시지는 필수로 써줘야됩니다!
 
브랜치 만들고 해당 브랜치로 작업환경(Working tree) 옮기기
> git branch 브랜치명
> git checkout 브랜치명

원격 저장소 등록하기
> git remote add origin 레포지토리주소a
> origin이라는 이름으로 원격 레포지토리 주소가 등록됩니다.

원격 저장소와 내 로컬저장소 연동(내 현재 로컬브랜치가 원격저장소에 없을 때)
> git push -u origin 브랜치명
> 한번만 원격저장소와 연동해주면 그 뒤로는 git push만 해주면 됩니다!
로컬 브랜치의 변경 사항
   

원격 브랜치의 변경 사항
     
 feature/류이서
