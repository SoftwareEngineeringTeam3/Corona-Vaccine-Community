#                                         소프트웨어 공학 팀3-3 (Use Case Diagram 보완:  include/extend + Use Case Description + Scenario Description + Activity Diagram)



**팀장** 고경환<br/>
**팀원** 박재홍, 이화영, 정우엽, 정주은

# Index

1. Project Title
2. Motivation
3. Competitive Technology Analysis
4. Main Functions
5. Participants Table
6. Use Case Diagram (include/extend 포함)
7. Use Case Description
8. Activity Diagram
9. Secinario Description

## 1. Project title 

**코로나 백신 커뮤니티(CVC, Corona Vaccine Community)**

## 2. Motivation

![img](https://lh6.googleusercontent.com/YJdjSwgyY4YyI8C28-FBw8ChCs4k40VveY7Db1wsIoMA-ZwJdG87plj5shQaKkQ-aUKknxRlKUEnspei5XYOzkS_ffhETGur9bP6A_qM2hHQWk8wTOVlRz89rteDTgqrIM8Df-qYrko=s0)

<div style="text-align:center">(출처: https://corona-live.com, 근 6개월간 월별 코로나 확진자 수(좌)</div>
<div style="text-align:center"> 출처: https://www.who.int/health-topics/coronavirus#tab=tab_2, WHO의 코로나 예방을 위한 백신 접종 권장(우)) </div>

+ 코로나 확진자 수의 지속적인 증가
+ 백신의 필요도 및 관심도 증가 

![img](https://lh5.googleusercontent.com/X45oD62jFTQxc105iOmJE2rp13mdubfxl9W_NRhH2k9lhVzY6kPQk4P2pquGzN3sAT1Vtfb9Jyw78DC5RQeA9IY8pec1d_c9MTQA8kOlsPkNxn-dKK-AfiIv2JntDJzquYV6LtjWPV8=s0)

<div style="text-align:center">(출처: https://youtube.com, "코로나 백신 접종 후기" 검색결과 - 평균 조회수 약 130만회)</div>

+ 백신 접종예정자들의 백신에 대한 호기심과 두려움 증가

- 백신 관련 정보공유 커뮤니티 필요성 증가

## 3. Competitive Technology Analysis

### Existing product comparison table

<img src="https://lh6.googleusercontent.com/uaaLRKexEzMOufjA87IoyuvkycCYzSzo5L9VE4UtJic81BJhm7DEDLFyHsFLbfAAvSaptAj0qGslC94Mk5_9Ome5HPh9p9cIQecrsxNJsyYelzrhfKXxHQb7ubcTu7rBVtN-UyycEnU=s0" alt="img" style="zoom:67%;" />



## 4. Main Functions

1. 백신 접종완료자들의 정보(백신종류, 기저질환, 복용중인 약 등)를 통해 백신 접종예정자들 개개인에게 적합한 정보습득 가능
2. 구체적 커뮤니케이션 활성화
   + 백신 접종완료자(1차/2차), 접종예정자, 전문 의료인 인증을 통해 분류
   + 댓글/대댓글을 이용해 실시간 소통가능
   + 좋아요 및 댓글 수를 통해 인기글 상단에 배치
3. 라이브 톡을 통한 접종완료자와 접종예정자간의 실시간 소통가능

4. 백신 관련 뉴스 및 기사 실시간 업데이트



## 5. Participants Table

| Participant | Roles                      | Skills                                  | Training needs           |
| ----------- | -------------------------- | --------------------------------------- | ------------------------ |
| 고경환      | Team leader                | HTML5, CSS, JavaScript, Reactjs, Python | UML, Communication Skill |
| 박재홍      | Data Collection & Analysis | Python, R, Django, Flask                | DB(MySQL), Java, UML     |
| 이화영      | FrontEnd Design, Tester    | Python, C, Java, HTML5, CSS             | Boot-Strap, UML, UI/UX   |
| 정우엽      | Configuration Manager      | Java                                    | Python, DB               |
| 정주은      | Market Research            | C, Java, Android Studio, HTML5, DB      | Python, DB, UML          |



## 6. Use Case Diagram (Requirement Eliciation, include/extend 포함)[1저자(고경환) 2저자(이화영)]

![img](https://lh6.googleusercontent.com/EjWEuTcBsaABjWW4xVIfVKXa-rOXcZHv1EnW_Z2lZMMbYQpWquZ26w66YG30ZCoXmZXL_SQifori462gLu7mDRlN_lNPTwUaLJKcjmJdgA8YcZwBwR7Qd0rmuXe6i99HBkYfyUYIOAk)

※ 질병관리청(KCDC, Korea Centers for Disease Control and Prevention)

## 7. Use Case Description[1저자(이화영), 2저자(고경환)]

### Description of use case1

**use case name:** share experience and information

**participating actors:**

Initiated by Vaccination Completion Person

communicates with Vaccination Expectation Person, Medical Advisor

**flow of events:**

1. Vaccination Completion Person activates "share experience and information" through CVC.

   1-1. CVC recives the form submitted by Vaccination Completion Person and provides a community environment.

2. Vaccination Expectation Person participate in the community provided by CVC.

**Entry condition:** vaccination Completion Person **** has completed the vaccination certification.

**Exit condition:** Vaccination Expectation Person get the information they need.



### Description of use case2

**use case name:** ask and answer question

**participating actors:**

Initiated by  Vaccination Expectation Person

communicates with vaccination Completion Person, Medical Advisor

**flow of events:**

1. Vaccination Expectation Person activates "ask and answer question" through CVC.

   1-1. CVC forwards the form that submitted to CVC by Vaccination Expectation Person to Vaccination Completion Person.

2. vaccination Completion Person answers the questions of the prospective Vaccination Expectation Person , and additional mutual questions and answers are made.

3. Vaccination Expectation Person get the information they need.

**Entry condition:** Vaccination Completion Person has completed the vaccination certification.

**Exit condition:** Vaccination Expectation Person get the information they need.



### Description of use case3

**use case name**: show vaccine related articles and news

**participation actors**: 

KCDC API, Vaccination Expectation Person

**flow of events**:

1. KCDC API provides CVC with vaccine-related articles, news, etc.

   1-1. CVC displays vaccine related articles and news.

2. Vaccination Expectation Person check vaccine-related articles and news provided by CVC.

**Entry condition:** Each vaccine-related article and news are uploaded to CVC through API.

**Exit condition:** Vaccination Expectation Person can check various vaccine-related articles and news.



### Description of use case4

**use case name**: verify vaccination

**participation actors**: 

initiated by Vaccination Completion Person

verify vaccination by Verification Server

**flow of events**:

1. Vaccination Completion Person enters his or her information to confirm his or her vaccination

   1-1. .CVC delivers information on the to Vaccination Completion Person Verification Server.

2. Verification Server recognizes the information of the Vaccination Completion Person provided by CVC, It gives approval that the vaccination has been completed.

**Entry condition:** Vaccination Completion Person enters their vaccination information.

**Exit condition:** Vaccination Completion Person is certified by Verification Server.



### Description of use case5

**use case name**: describe existing condition

**participation actors**: 

initiated by Vaccination Completion Person

Vaccination Expectation Person get information

**flow of events:**

1. Vaccination Completion Person enters information such as what underlying diseases he or she is suffering from and what medicines he or she took.

   1-1. CVC delivers information of Vaccination Completion Person to the Vacation Expection person.

2. The Vacation Expression Person obtains information such as the underlying diseases and medication of the Vacation Completion Person provided by CVC and compares it with his or her case.

**Entry condition:**

Vaccination Completion Person enters information such as his or her underlying disease and taking medicine.

**Exit condition:**

Vaccination Expectation Person can obtain information such as underlying diseases and medication of those who have already been vaccinated and compare them with their own cases.



## 8. Activity Diagram[1저자(박재홍), 2저자(고경환)]

### Flow of event about "ask and answer question"

![img](https://lh5.googleusercontent.com/7SsH7Q4PQYpeRyaMH0TQra8cHDcuxz2oUbKfpoPsESrqoI0VP18xe_PyQ4Yi_YvnzC9TE1gu7MAbXThvmbSqU2uBuwBlaXCdzVKmmGuQMEHHoMwuCe6qZ7PSnWWqEkjMwFDuNQVyyMk)



### Flow of event about "verify vaccination"![img](https://lh4.googleusercontent.com/GW42-L7jOeOQfXOG15Lj-_ALm6OBabSC7MiksoLcHKZIE9N0sfp684VYIY6n89jImhyWXTSYEFAyaLTL_ohTik-TsOEBzuJf8EBf-SnaJzPWfIui0xaqWDydOkr_C3KFpiwDgVC3qNA)



## 9. Secinario Description[1저자(정우엽, 정주은) 2저자(고경환)]

### Scenario name: <u>Get information about current situation: show vaccine-related articles and news</u>

Participating actor instances :

- <u>정우엽(Pfizer) : Vaccination Completion Person</u>
- KCDC API

Flow of events :

1. 정우엽 accesses CVC.
2. KCDC API  pop-ups the related articles and news.
3. KCDC API pop-up the number of people infected with Corona the previous day and an articles related to government measures.
4. KCDC API shows the supply and demand for vaccines.
5. KCDC API shows the status of vaccine-related side effects and deaths.
6. KCDC API shows the identification of the specific numbers of primary and secondary immunizations.
7. 정우엽 became aware of the general situation outgoing.



### Scenario name: <u>Get Vaccination Certified: verify vaccination</u>

Participating actor instances :

- <u>정우엽(Pfizer) : Vaccination Completion Person.</u>
- <u>정주은 : Medical Advisor</u>
- <u>박재홍 : Vaccination Expectation Person</u>
- Verification Server

Flow of events :

1. Verification Server process the implementation of vaccination completion certification.
2. 정우엽 captures and uploads the inoculation certificate through KakaoTalk in order to verify his inoculation record (Pfizer, 2021.10.02) and Verification Server verifies and approves.
3. In order to certify that she is a medical professional, 정주은 presents her employee ID, and the Verification Server confirms and approves it.
4. 박재홍 didn't present anything, the verification server classifies him as a vaccination expectation person.
5. 정우엽, 정주은, 박재홍 were able to clarify who they are within the site.



### Scenario name : <u>Posting after vaccination : share experience and information</u>

Participating actor instances :

- <u>정우엽(Pfizer), 고경환(Pfizer), 이화영(AZ) : Vaccination Completion Person</u>
- <u>박재홍 : Vaccination Expectation Person</u>

Flow of events :

1. Sharing 정우엽's vaccination experience and side effects.
2. 정우엽 wrote a post saying that he had been vaccinated at a nearby internal medicine, had a little longer waiting for vaccination, and that the vaccination process was virtually no different from getting a preventive injection.
3. In the case of 정우엽, although the vaccination was completed, he had asthma and anaphylaxis. In addition, since He is allergic to Cefa antibiotics, ibuprofen, and penicillin, He write about the medications he took and his experiences after vaccination on CVC.
4. 정우엽 wrote a post saying that he was okay immediately after getting vaccinated, but his arm hurt very much the next day, had a fever, and gradually began to improve three days later.
5. 정우엽 wrote that he took acetaminophen-based tyrenol, not a Brufen-based antipyretic because his arm hurt.
6. 고경환 wrote an answer that he was not sick at all and had no side effects.
7. 이화영 wrote that she felt a strong pain in the area of headache and vaccination.
8. 박재홍 confirms this before his vaccination.



### Scenario name : <u>Ask a question about Pfizer Vaccines: ask a question</u>

Participating actor instances :

- <u>박재홍(Pfizer) : Vaccination Expectation Person</u>

Flow of events :

1. Before 박재홍 was vaccinated, he posted to know the side effects and necessary things.
2. Waiting for answer



### Scenario name : <u>Answer a question about Pfizer Vaccines: answer a question</u>

Participating actor instances :

- <u>정우엽(Pfizer), 고경환(Pfizer) : Vaccination Completion Person</u>
- <u>박재홍(Pfizer) : Vaccination Expectation Person</u>
- <u>정주은 : Medical Advisor</u>

Flow of events :

1. 정주은 looks at the question that posted about Pfizer vaccines by 박재홍.
2. 정주은 writes a specific answer to 박재홍's question.
3. 고경환 and 정우엽 write answers to 박재홍's questions based on their experiences.
4. 박재홍 is checking the comments.
5. Additionally, 박재홍 collects information using popular posts.
