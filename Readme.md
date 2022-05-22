✅
node-sass src/style.scss dest/style.css
src/style.scss를 dest/style.css로 바꿔줘!

✅
"sass": "node-sass styles/main.scss ./style.css"
input: design/styles/main.scss
output: design/styles/style.scss

✅
watch a directory or file
-w, --watch : 어떤 변경사항이 있는지 파악하겠다.
recursively watch directories file
-r, --recursive : 어떤 파일이 변경 사항이 있는지 파악한다.

✅
- Usage
  node-sass [options]<input>[output] Or: cat<input> | node-sass > output
  "sass": "node-sass -w styles/main.scss ./style.css"
  "sass": "node-sass -w -r styles/main.scss ./style.css"
  "sass": "node-sass -wr styles/main.scss ./style.css"



