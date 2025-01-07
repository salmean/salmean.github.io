## 초기 설정
1. git 회원가입 및 다운로드
2. 바탕화면에서 오른쪽 마우스를 눌러 'open git bash here' 클릭
3. 원하는 위치에 git 폴더 생성 후 이동
4. 내 기준 git clone https://github.com/salmean/salmean.github.io 입력
5. - git config --global user.name "github 아이디"
   - git config --global user.email "github 이메일주소"
     를 입력해준다.

## 로컬에서 파일 업로드
1. 생성한 git 폴더에 업로드할 파일 넣기
2. 바탕화면에서 오른쪽 마우스를 눌러 'open git bash here' 클릭 후 bash에서
   - git add -A(모든 내용) / git add 파일명.확장자(특정파일) 입력
3. git commit -m "first commit" (뒷 멘트는 업로드 정상 확인용이라 아무렇게 써도 됨)
4. git push (저장소 업로드)
5. 'sign in with your browser'를 누르면 브라우저 팝업이 뜨고 'Authorize GitCredentialManager'를 누르면 업로드가 완료된다.
