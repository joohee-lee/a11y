# a11y
a11y test


# IOS 14.~ 
## Voiceover  이슈 정리 
### 1. 가상 포커스 상태, CTA 요소 포커스 상태 
    
### 2. SVG 를 img 요소 엘리먼트를 사용하여 적용할 경우, css display(flex, float, position... ) 배치요소를 적용하여 작업한경우
 - 문제 : 텍스트로 인식하기때문에  "이미지" 라고 읽거나, title 이 적용되어 있으면 svg title 를 읽는 현상 발견. 
 - 해결 : 현 소스 상태에서는  img src="icon.svg" role="img" 로 지정하거나 마크업 케이스에 따라 적당한 wai-aria role 을 지정하여 해결하나. 
          블릿의 성격이나 무의미한 성격의 svg 요소라면 css 로 디자인을 한다. 
          
  
### 3. label + input text 형식일 경우, id와 for 값으로 연결하게 되면 
    `
    IOS 16 이슈 

    lable + input-text 조합에서는 id for 연결 생략 
    lable + input-text for + id 연결시, label focus 가 가질 않음. 
    그러나, <label for="a"> text <span>*</span></lable><input text="" id="a"> 이런경우는 lable 안에 focus 발생.
    
    문제가 크게 되지 않으니 lable + input text 조합시에는 id for 연결 생략 
    
    ex) input.html
    `
