# 협업과 개발을 원활하게 하기 위해 이 파일을 계속 편집할 예정이므로 수시로 확인할 것!

# 개인별 branch 생성후 작업한 뒤 github repo에 push 및 PR 요청

## git status 상태 정리

### 1. branch에서 작업한 뒤 add를 하지 않으면 git status시 파일명이 빨간색(modified 파일명)으로 표시됨 => git add . 진행  ( .은 'all'의 의미, 즉 모든 파일에 대해 ~)

# [git branch 전략]
한번씩 아래 링크와 진영님이 정리해놓으신 git flow 내용 읽고 작업하기.
git flow:  https://techblog.woowahan.com/2553/ 
### 2. add 후에는 git status시 파일명이 초록색(midified 파일명)으로 변경 됨 => git commit -m "commit message 내용" 진행 ex) git commit -m " ADD: 로그인 페이지 레이아웃 구현 완료"

## [commit convention]

1. Add: 코드나 테스트를 추가했을 때 <br>
2. Fix: 버그를 수정했을 때 <br>
3. Remove: 코드를 제거했을 때 <br>
4. Update: 코드보다는 문서나 라이브러리 등을 보완했을 때 <br>
5. Docs: 문서를 수정했을 때 <br>
6. Style: 코드 포맷팅에 대한 부분 변경, CSS 변경 등<br>
7. Rename: 이름을 변경했을 때 <br>
8. Move: 코드를 이동할 때 <br>
9. Refac: 코드 리팩토링 <br>
10. Test: 테스트 코드 수정 <br>
11. Chore: 그 외 자잘한 수정 <br>

예를 들어, 로그인 기능에 대한 버그를 수정했다면 git commit -m "Fix: Login bug " 이런 식으로 작성해서 팀원들이 어떤 작업을 수행했는지 서로 확인하기 쉽게 commit message를 
일관성 있게 작성해주세요!

### 3. git log ( git log로 commit 내역 확인 수시로 합시다! )

### 4. 커밋 내역을 확인하였다면 local에서 작업한 branch를 remote로 push => git push origin 브랜치명 ( git clone을 통해 저장소를 복제 했다면 일반적으로 origin이 원격 저장소입니다. git push origin 브랜치명은 브랜치에 남겨놓은 코드 commit 내역을 origin 원격저장소에 올리겠다는 의미입니다.
### 4. Github Repo에 가서, PR request 템플릿에 맞게 작성 후, 리뷰 요청

## Push 하기 전 검토해야할 사항

- github에 push 한 뒤 conflict 사항을 확인하기 보다 push 하기 전 최신의 main 코드를 merge하여 conflict를 해결한 뒤 push를 하는 것이 현명합니다.
(1) git add, commit
(2) git checkout main(master)
(3) git pull origin main(master)
(4) git checkout feature
(5) git merge main(master)
(6) (컨플릭트 발생 시 해결 후 add, commit)
(7) git push origin feature

conflict 관련 내용 혹시 이해가 되지 않는 부분이 있다면 편하게 물어봐주세요! 그리고 인터넷에 자료도 많으니까 검색하면 아마 해결하실 수 있으실 것 같습니다.

<출처> wecode(코딩 부트캠프) 세션

-----------------------------------------------------------------------------

## 빌드 및 실행 방법

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
