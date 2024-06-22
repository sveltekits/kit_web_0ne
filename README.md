# 서브릿 설치
```
npm create svelte@latest my-app
```

# TailwindCss 설치
```
1. npm install -D tailwindcss postcss autoprefixer
2. npx tailwindcss init tailwind.config.cjs -p
--> Created Tailwind CSS config file: tailwind.config.cjs
--> Created PostCSS config file: postcss.config.js

3. tailwind.config.cjs 파일 내용 변경
    export default {
        content: [],
        ==> content: ['./src/**/*.{html,js,svelte,ts}'],
        theme: {
            extend: {}
        },
        plugins: []
    };
4. src/app.css 생성
    @tailwind base;
    @tailwind components;
    @tailwind utilities;

    // vscode에서는 플러그인 PostCSS Language Support를
    // 설치하면 더 이상 경고 문구가 보이지 않는다

```
# 폰트 사용
```
1. 구글사이트에서 폰트 css 가져와서 app.html에 붙여 넣음
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
2. 아이콘 사용 : fontawesome cdn 가져옴
    [ https://cdnjs.com/libraries/font-awesome ]
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
```