🏃 GodSang 프로젝트를 소개합니다 🏃‍♂️
==================================

### Want to live a productive and fulfilling life?    Start your ‘GodSang’ journey with us today!
#### 성실하고 보람찬 삶을 살고 싶으신가요? 지금 바로 우리와 함께 ‘갓생’ 여정을 시작하세요!
---------------------------------

갓생’은 젊은 세대 사이에서 시대적 트렌드 입니다.   
신을 뜻하는 ‘갓(God)’과 인생을 뜻하는 ‘생(生)’의 합성어로 입니다. 생산적 활동으로 하루를 채우는 삶을 의미합니다.     
갓생 프로젝트는 생산적인 삶을 지향하는 사람들을 돕는 어플 구현을 목표로 합니다.       

## 🛠️기능 구현

> 1. 레시피 기능 제공    
>   > 식단별로 카테고리화 되어 다양한 건강한 레시피를 제공   
또한 원하는 재료를 사용하여 요리하고 싶을때 검색창에 입력하면 해당 재료를 사용하는 레시피를 사용자에게 제공  
> 2. 운동 기록 기능 재공
>   > 운동의 종류를 헬스/홈트레이닝/기구활용여부 등 다양한 장르로 나누어 운동명과 운동량을 기록하는 기능을 제공     
하루에 얼마나 어떤 운동을 어떤 비율로 했는지 사용자가 가시적으로 볼 수 있도록 원형그래프 제공   
운동 안전 가이드 제공
> 3. 냉장고 기능
>   > 냉장고에 있는 식품의 유통기한/소비기한을 기록   
사용자가 유통기한이 임박한 제품부터 볼 수 있도록 정렬하여 빠르게 냉장고 정리가 가능하도록 구현   7일전 / 3일전 / 하루전 / 당일 유통기한/ 소비기상 알림 서비스 제공 예정

## ⚙️ 기능 명세서

1. 식단 카테고리화 - UITableViewDataSource, UITableViewDelegate, UItable view 를 사용하여 테이블 뷰의 데이터를 관리하고 셀을 생성 및 구현

2. 재료와 음식 이름 검색 - UISearchResultsUpdating

3. 선택한 음식의 레시피와 사진을 전달하여 새로운 화면에 띄우는 기능 - segue

4. 운동의 이름과 운동 시간을 저장 - sigleton class를 사용하여 변수 : 타입 배열 형태로 누적 시간을 구함

5. 운동 시간 기록 - UIDatePicker 를 사용하여 시작 시간과 끝나는 시간을 기록

6. 원형그래프 작성 - 싱글톤 클래스에 저장된 운동명:운동시간 배열을 바탕으로 PieChartView 메서드로 작성

7. 날짜 데이터를 받아 문자열로 변환 후 테이블뷰로 이동 - DateFormatter 사용, string(from:) 메서드를 호출, 업데이트 후 식별자를 사용하고, dequeueReusableCell를 통해 재사용 가능한 셀을 가져옴

## 📱결과물
 * [GodSangLife 프로젝트 다운로드](https://github.com/hyun2eee/GodSangLife/blob/main/GodSangLife/GodSangLifeProject.xcworkspace.zip)

## ➿기술 스택
> * Swift, Storyboard 기반 개발

## 💡플로우차트
<img width="417" alt="img1" src="https://github.com/user-attachments/assets/8477b4e4-612f-4dec-82f2-f172121a8e15">  

앱의 주요 동작을 설명하는 플로우 다이어그램

## 🔌실제 구현 화면
<img width="419" alt="img2" src="https://github.com/user-attachments/assets/6c1c0537-424b-44a8-85f5-88f50cf38762">   

레시피 검색 화면과 운동 기록 화면   

사용자 친화적인 인터페이스로 간결하고 직관적인 디자인을 채택했습니다.

## ⚒️추후 추가 내용 및 수정사항

1. 냉장고 알림 기능 추가 : 유통기한이 임박한 식품에 대해 사용자에게 푸시 알림 제공
2. 레시피 추가
3. 레시피 선택시 이미지 첨부

> 위 프로젝트는 개인으로 진행된 프로젝트 입니다.