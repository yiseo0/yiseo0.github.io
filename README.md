# 깃허브 블로그 생성 + Jekyll를 이용한 테마 적용
<br>

## 🌱 **깃허브 블로그 만들기**


1.  **사용자이름.github.io 레포지토리를 생성한다.**
    
    *ex)사용자 이름이 yiseo0일 경우 yiseo0.github.io*
    <br><br>

2. **만든 레포지토리에 index.html 파일을 추가**

   index.html 파일을 추가하면 [https://yiseo0.github.io](https://yiseo0.github.io) 접속이 가능해진다.
 
   index.html 파일에 코드를 작성하여 나만의 블로그를 만들 수 있다 🙂<br><br><br>


## 🌱 **깃허브 블로그 테마 적용하기**

**Jekyll라는 정적 웹사이트 생성기**를 이용하여 테마 적용하기
   
   Jekyll는 ruby(루비)라는 프로그래밍 언어로 만들어져서 **Jekyll 사용하려면 ruby를 설치해야한다.** <br><br>



### 1. **ruby 다운로드 및 설치 [https://rubyinstaller.org/downloads/](https://rubyinstaller.org/downloads/)**

           
         💡 Jekyll는 32bit 이기 때문에 ruby도 반드시 32bit로 설치해야 한다.
         또한 Devkit를 사용하기 때문에 포함되어 있는 파일로 다운로드 해야한다.
         ex) Ruby+Devkit 3.1.3-1 (x86) 

           

   루비 버전이 정상적으로 나오는지 확인

   ```jsx
   cmd) ruby -v 
   ```   
 <br>
 
### 2. **루비 라이브러리 패키지로 jekyll bundler 설치** 

   ```jsx
   cmd) gem install jekyll bundler
   ```
   <br>
   
### 3. **레포지토리 안에 있는 파일들(index.html, READM.md) 전체 삭제** 

   *삭제하지 않으면 오류 발생

   <br>
   
### 4. **jekyll를 이용한 사이트 생성** 

   cmd에서 레포지토리 경로로 이동하여 하단 명령어 실행

   ```jsx
   cmd) jekyll new ./
   ```
   <br>
   
### 5. **Jekyll 서버를 로컬 컴퓨터에서 실행하여 확인**

   ```jsx
   bundle exec jekyll serve
   ```

   [http://127.0.0.1:4000/](http://127.0.0.1:4000/) 로컬 서버에서 확인 가능
    <br><br>
    
### 6. **마음에 드는 테마를 찾고 적용하기**
    
테마는 fork하여 bundle install로 적용하는 방법과 zip 파일로 다운받아 덮어 씌우는 방법이 있다.

간단하게 덮어씌우는 방법으로 적용해보자 🙂<br><br>


  **(1) 테마 다운로드 받기**

  다양한 테마가 많으니 마음에 드는걸로 찾아보자. 나는 하단의 테마를 적용할 예정이다.

  [https://github.com/hydecorp/hydejack-starter-kit](https://github.com/hydecorp/hydejack-starter-kit)<br><br>

  **(2) 레포지토리에 _config.yml 파일이 있는 경로에 전체 파일을 덮어씌운다.**  
  **(3) Jekyll 서버를 로컬 컴퓨터에서 실행하여 테마가 변경된 것을 확인한다.**

  ```jsx
  cmd) bundle exec jekyll serve
  ```
  <br>

  **(4) 해당 내용을 푸쉬하면 나의 블로그 주소([https://yiseo0.github.io](https://yiseo0.github.io))에서 테마가 변경된 것을 확인 할 수 있다.** 
