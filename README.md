# markdown_29230127
마크다운 설명

### 프로젝트 readme.md
1. 주제  
  SOLAR EMBASSY
  motive by Lunar Embassy & DCinside & inven
2. 기획  
  태양계 컨셉의 종합 커뮤니티 사이트 개발  
3. 설계  
  유저 등급 및 화면 디자인을 통한 컨셉 반영  
4. 테스트  
  유닛테스트 > 시스템테스트 > 통합테스트 > 인수테스트  
5. 시연  
  
### 11. 표
|번호|아이디|이름|레벨|이메일|등록일|
|:--|:----|:-- --|-:|:---------------|:--------:|
|1  |james|이상무1|1|jamesol@paran.com|2023-01-27|
|2  |james|이상무2|1|jamesol@paran.com|2023-01-27|
|3  |james|이상무3|1|jamesol@paran.com|2023-01-27|
|4  |james|이상무4|1|jamesol@paran.com|2023-01-27|
|5  |james|이상무5|1|jamesol@paran.com|2023-01-27|
|6  |james|이상무6|1|jamesol@paran.com|2023-01-27|

### 10. 인라인
문단 중간에 `CODE`를 넣을 수 있습니다.  (고정 폭 폰트를 표시해야 할 때 사용)
예를 들어 `question_list=Question.objects.order_by('-create_date')`처럼


### 9. 강조
**Spring**을 만끽하세요.  
*Spring*을 만끽하세요.

### 8. 이미지 넣기
![사과](doc/사과.jpg "사과")


### 7. 하이퍼 링크
[e클래스](http://cafe.daum.net/pcwk "e클래스의 cafe입니다.")


### 6. 가로 라인
---
***
------

### 5. 코드블록
```
def index(request):
    """question list"""
    # list order create_date desc
    question_list = Question.objects.order_by('-create_date')  # order_by('-필드') desc,order_by('필드') asc
    # question_list = Question.objects.filter(id=99)
    context = {'question_list': question_list}
    print('question_list:{}'.format(question_list))
    return render(request, 'pybo/question_list.html', context)
```


### 4. 목록
1. 아이템1
2. 아이템2  
  9. 1단계 하위 아이템  
    3. 2단계 하위 아이템
9. 아이템3

- 아이템 1  
+ 아이템 2  
  - 1단계 하위 아이템  
    * 2단계 하위 아이템  

순서없는 목록  
* 목록이름
- 목록
+ 목록

순서 있는 목록
1. 목록이름
2. 목록
3. 목록3번

### 3. 인용문
> 여기에 인용할 내용을 넣으면 됩니다.  
> 빈 줄이 없으면 자동으로 인용 상자에 포함이 됩니다.

### 2.헤더
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5

### 1. 문단 구분을 위한 개행.
문단을 작성합니다.(개행 공백 2개)  
겨울이 가고 봄이 옵니다.
