# edifileTdd
restdocexample
기존에 상태는 
edi 파일이 들어오면  각각의 분리된 TAG에서 
다이렉트로 DB에 저장을 하는 구조로 되어있다.

하지만 이럴경우 새로운 컬럼이 추가되거나  코드가 변경되었을시
테스트하기가 굉장히 어려운 경우가 있다.

그래서 EDI 파일만 읽는 로직과  , 그것을 가공하는 로직 , 분리후 
VO 로 담은 후  
DB에서 데이터를 처리하도록 구상을해보았다 

해야될것들
- EDI 분리 태그  그룹마다 각각의 테스트를 작성해보기 
