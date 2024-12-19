### Git 서브모듈 사용법 📚

#### 1️⃣ 서브모듈이란?

- Git 저장소 안에 또 다른 Git 저장소를 포함하는 기능
- 큰 프로젝트에서 외부 라이브러리나 독립적인 코드를 포함할 때 사용

------

#### 2️⃣ 서브모듈 추가하기

```
git submodule add <저장소 URL> <디렉토리 이름>
```

- 예

  ```
  git submodule add https://github.com/example/library.git libs/library
  ```

- 디렉토리 이름을 생략하면 기본적으로 저장소 이름이 사용됨

------

#### 3️⃣ 서브모듈 초기화 및 업데이트

- 서브모듈을 다운로드하거나 최신 상태로 동기화

```
git submodule update --init --recursive
```

------

#### 4️⃣ 서브모듈 상태 확인

- 서브모듈의 상태를 확인

```
git submodule status
```

------

#### 5️⃣ 서브모듈 변경사항 반영

1. 서브모듈 디렉토리로 이동

   cd <서브모듈 경로>

2. 작업 후 변경 사항 커밋

   ```
   git add .
   git commit -m "Update submodule"
   git push
   ```

3. 메인 저장소에서 서브모듈 커밋을 반영

   ```
   git add <서브모듈 경로>
   git commit -m "Update submodule reference"
   git push
   ```

------

#### 6️⃣ 서브모듈 삭제하기 ❌

1. 서브모듈의 추적 제거

   ```
   git rm --cached <서브모듈 경로>
   ```

2. 디렉토리 삭제

   ```
   rm -rf <서브모듈 경로>
   ```

3. `.gitmodules` 파일에서 해당 항목 삭제

4. 변경 사항 커밋

   ```
   git commit -m "Remove submodule"
   ```