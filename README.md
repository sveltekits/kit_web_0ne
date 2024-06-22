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
