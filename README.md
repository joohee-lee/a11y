# a11y
a11y test


# IOS 14.~ 
## Voiceover  이슈 정리 
### 가상 포커스 상태, CTA 요소 포커스 상태 
    
### SVG 를 img 요소 엘리먼트를 사용하여 적용할 경우, css display(flex, float, position... ) 배치요소를 적용하여 작업한경우
 - 문제 : 텍스트로 인식하기때문에  "이미지" 라고 읽거나, title 이 적용되어 있으면 svg title 를 읽는 현상 발견. 
 - 해결 : 현 소스 상태에서는 <img src="" role="img"> 로 지정하거나 마크업 케이스에 따라 적당한 wai-aria role 을 지정하여 해결하나. 
          블릿의 성격이나 무의미한 성격의 svg 요소라면 css 로 디자인을 한다. 
          
  
