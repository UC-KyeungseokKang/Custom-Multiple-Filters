# Custom-Multiple-Filters


 Custom-Multiple-Filters using Google Cloud NLP API & Boolean IR
 
 
 ## implement process
 
1.웹사이트에서 데이터를 크롤링하여 테스트 사이트 구현

2. 각 키워드가 포함된 게시글 100개씩 추가 생성

3. 멀티 필터링 기능 구현

4. 멀티 필터링을 이용하여 전체 목록 중에서 원하는 글이 찾아지는지 확인( Boolean IR)

5. 찾아진 글에서 미리 설정한 감정 값 범위에 따라 필터링이 되는지 확인( Sentiment filter)


![image](https://user-images.githubusercontent.com/38004643/59550078-7d86be80-8fa1-11e9-9f62-086fa26465cb.png)


## Filtering Result (Keyword = 페미, 씨발)
 <KEYWORD_페미_ filtering >
 
1 :  간호는 여초인데도 - 페미세력 거의없거든 근데 씨발 여초페미인냥 까대는거 너무 같다  개씨발 페미년들때문에 뭔난리냐58 : 페미들 발광하는거 너무 재밌어 - 얼마나 쳐맞어야 쥐죽은듯 지내려나 쓰래기들

71 : 오냐오냐 해주니까 아주 병 난게 페미아니냐 – 여자라고 이해해주고 배려해주니까 지랄 똥들을 싸고있네


 <KEYWORD_페미_ No filtering>
 
6 :  산이근황 - 이게 페미니즘이다 말이야

48 : 우파인 여자만나면 80프로 페미거르는거시야 - 우파인 남자 만나면 80프로 최대일베 최소 야갤인거시야

99 : 솔직히 페미들 앞에서 페미편듬 - 그렇다고


 <KEYWORD_씨발_ filtering>
 
1 :  간호는 여초인데도 – 페미세력 거의없거든 근데 씨발 여초페미인냥 까대는거 너무 같다  개씨발 페미년들때문에 뭔난리냐

8 :  아니 시발 레벨 공연때 응원봉던진새키누구냐– 진심 존나 빡쳤었던게 중간쯤에서 응원봉 레벨한테 던짐  맞기라도 했으면 진짜

40 : 씨발– 씨발

 <KEYWORD_씨발_ No filtering>
 
11 : 레드벨벳 봐서 좋은데 - 내일 1교시 실화냐 으아아아악그 후에는 학원알바그 다음날은 편의점 스바씨파

48 : 에타 진짜 - 씨발이네 

99 : 근데 페시발은 진짜 - 페시발은 진짜 너무했다사회자랑 이거랑 묶여서 지금 밖에서 중앙대 수준 낮다고 욕 먹는다.

![image](https://user-images.githubusercontent.com/38004643/59550137-567cbc80-8fa2-11e9-900e-7fce21b96cf6.png)

