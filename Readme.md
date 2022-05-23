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


✅
(선)jpg === (후)jpeg 호환가능


raster image vs vector image
확대할때 깨진다 -> raster image(jpg, png 권장)
확대할때 깨지지 않는다 -> vector image(svg 권장)

✅
이미지의 용량이 크다. -> 웹사이트의 로드가 느려진다 -> 사용성이 구리다
프론트엔드 개발자는 퍼포먼스에 해를끼치는 요소를 없앨 줄 알아야 한다.
raster image -> jpg vs png

1. 투명 배경 지원

jpg: 투명 배경 지원하지 않는다
png: 투명 배경을 지원한다.

2. 이미지 압축 방식

jpg: 압축이 잘된다 (용량이 적다) -> 압축이 될 수록 이미지의 퀄리티가 떨어진다.
png: 압축이 잘안된다 (용량이 크다) 압축이 될 수록 이미지 퀄리티가 크게 떨어지지 않는다.

어떻게해야해?

- 퀄리티의 품질에 따라서 이미지를 정할 줄 알아야 한다.

3. webp
구글에서 만든 이미지 파일.




✅ Scalable vector graphics
- 아주 깔끔한 이미지 파일을 쓸 수 있다.
- 사이즈가 변경이 되더라도 일정한 디자인을 유지하고있다.
- font
- 용량이 다른 파일에 비해서 상대적으로 작은 편이다.
- 이미지 크기를 다르게 할 경우 png -> byte가 커진다. svg -> 일정한 크기를 유지한다.

bitmap -> 픽셀 크기가 많아진다면 용량이 커진다
vector -> 크기를 유지한다.

Logo, Icon -> SVG




svg 사용하는 방법
1. img tag에 src를 입력하는 방법
2. css Background로 사용하는 방법
3. svg 사용하는 방법
currentColor -> 부모 Color를 상속받을 수 있다.
<svg width="24" height="25" viewBox="0 0 24 25" fill="currentColor" xmlns="http://www.w3.org/2000/svg">

4. svg파일 최적화 하는 방법
icomoonApp 접속 -> import -> 하단 Navigation 오른쪽 하단-> 다른거 설정 필요없이 select를 i로 변경 -> 다운롣,ㅡ