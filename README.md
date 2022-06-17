# GITBASH

###  명령어 

- ls -al ( 중간에 spacebar 꼭) : 어떤 파일들이 있는 지보여주는 명령어
- ls - 해당 디렉토리의 폴더 상세정보 출력
- cd <폴더명> (<> 는 가독성상 넣은거지 명령어엔 사용x) : 폴더로 이동하는 명령어
- cd .. : 이동했던 폴더에서 뒤로 나오는 명령어
- mkdir <폴더명> : 빈 파일을 바로 생성하는 명령어
- rm - rf <폴더명 또는 파일명> : 폴더 또는 파일을 지우는 명령어
- mv <이전폴더명> <변경할 폴더명> : 폴더 / 파일명 변경 

# markdown 필기

### Heading(#)

- `#` 해시태그의 개수만큼 헤딩의 중요도가 결정됨.
- `h1` ~`h6` 태그가 있음



### List(1, *, -)

#### 순서가 있는 리스트

1. 하나
2. 둘
3. 셋
4. 넷!    

- `숫자` +`.` 으로 작성 가능

### 순서가 없는 리스트

- 이거
- 저거
- 그거
- 요거
- `*/-` +`space bar` 으로 작성 가능



###  Code Block

오늘 배운 내용

사용법

- `ctrl` `shift` `k` 로 생성

```python
import time

time.sleep(60)
print('안녕 여러분?')
```

- `빽킷`*3 -> 코드 블럭
- `빽킷` *2 -> 인코드 블럭



### Link

[네이버](https://www.naver.com)
[구글](https://www.google.com)

- `[텍스트]` `(링크)` 
  - 링크로 이동하게 된다.



### Image

- ![이브이](README-images/ISTJ.png)

- `![텍스트]` `(링크)` 
  - 링크로 이동하게 된다.



### Text  emphasise

### **Bold**

- **노동영**
- **천승진**
- **신상연**
- **`텍스트`** 
- `ctrl` +`b`

### *Italic*

- *이수진*
- *박주영*
- *`텍스트`*
- `ctrl` +`i` 

### ~~Strikeout~~

- ~~오지혜~~
- `~~`텍스트 `~~` 

### Divider

___

---



- `_\-` *3

- HTML

  - `<br>`: 한줄 띄어주기
  - `<hr>`: 한줄  그어주기

  <hr>

### Blockquotes

> `>` 한개만 작성하면 인용문을 만들 수 있습니다.
>
> > depth 가 생깁니다.
> >
> > > depth가 또 생겼습니다.



### Table 

`|` (bar) : 선

`space bar` : 칸 

|      |      |      |      |
| ---- | ---- | ---- | ---- |
|      |      |      |      |
|      |      |      |      |
|      |      |      |      |

너비 조절은 안됨



# **Git - Github 연결 (User)**

### **한번만 해도 되는 작업**

`git config --global user.name <username>` :  username 등록

`git config --global user.name` :  username 확인

`git config --global user.email <email>` : email 등록

`git config --global user.email` : email 확인

# **Git - Github 연결 (Repository)**

### **⭐️Repository 연결할때는 한번만 해도 되는 작업⭐️**

`git init` : git 시작

`git remote add origin <git repository url>` : repository 연결

### **파일 수정, 생성, 삭제 할때마다 해야하는 작업!!! == 뭐든 할때마다**

`git add .` : 모든 파일 staging area에 올리기

`git add <file_name>` :  파일 staging area에 올리기

`git commit -m '<commit message>'` : 커밋 message 작성

`git push origin master` : github로 밀어내기!

`git pull` : github에서 로컬로 당겨오기!

# 6/16 수업 필기

- `git config --global user.name <user_name>` : username

- ```
  git config --global user.email <email>
  ```

   : email

  - config는 내 로컬과 깃헙 계정을 연결시켜줄 때 1회만!!!!

- ```
  git init
  ```

   : 레포를 만들고 워킹 디렉토리랑 연결시켜줄때 최초 1회

  - 레포 만들때마다!
  - 여러분들이 레포를 만들때마다 계속 해주셔야한다.

- ```
  git status
  ```

   : 워킹 디렉토리에 어떤 변화가 있는지 알아보는 명령어.

  - 워킹 디렉토리 단계와 스테이징 에리아 단계의 변화

- `git add` + `.` : 전체 다 staging area로 올리기

- ```
  git add
  ```

   \+ 

  ```
  파일명.확장자
  ```

   : 이것만 올려

  - ex) `git add 파일1 파일2 파일3`

- ```
  git commit
  ```

   \+ 

  ```
  m
  ```

  ```
  "commit message"
  ```

  - 되도록 명령어로 적기
    - 동사형으로 시작하기
    - 영어로 적기
  - 약속일뿐 법은 아니다.

- ```
  git log --oneline
  ```

   : `` (하이픈) 두개입니다.

  - `commit`된 상황에서 어떤 메시지로 언제 뭐가 올라갔는지 알기위한 명령어

- ```
  git remote add
  ```

   \+ 

  ```
  origin <github 주소>
  ```

   : 내 워킹 디렉토리와 레포지토리 연결

  - `git remote -v` : 리모트가 잘 들어갔는지 확인

- `git push` + `origin master` : 최종으로 깃헙에 올린다!!!

1. `git config --global user.name / email` 잘 적었는지 확인

2. ```
   git remote 확인
   ```

   - `git remote add origin <깃헙 주소>`

3. `git add` 했는지

4. `git commit` 잘 했는지 확인
