# TIL
이것도 MARK DOWN 형식을 이용한다.


---
Today I Learned
3일차 배운것

## 기술통계 (Pandas Profiling)
* 파이썬상에서 명령어 입력 후 프로그램을 다운로드 받아야함
* 런타임 다시 시작하기

### from pandas_profiling import ProfileReport
pandas_profiling 전체를 임포트를 안하고 거기에서
 profile report만 가져오는 이유는 성능 문제 인가요?

-> 사실 하드웨어가 매년 엄청난 성능 향상이 있는 현대에와서는 크게 의미가 없지만, 
	파이썬의 처음 발표일이 1991년이란걸 감안해보면... 
	왜 필요 했을지 바로 알 수 있는 부분이 있습니다.

## 단어 :
왜도값 (=비대칭도, skewness)
* 분포의 비대칭의 정도, 즉 분포가 기울어진 방향과 그 기울어진 정도를 나타내는 척도이다.
* 왜도는 실수 값 확률 변수의 확률 분포 비대칭성을 나타내는 지표이다. 
특잇값(singular value)
* 특잇값은 콤팩트 작용소와 그 에르미트 수반의 합성의 고윳값의 제곱근이다.
* 항상 양의 실수이다

이상치(Outlier)
* 패턴에서 벗어난 값
* 중심에서 좀 많이 떨어져 있는 값

편차(deviation)
* 관측값과 평균의 차이를 말한다
* 관측값에서 평균 또는 중앙값을 뺀 것이다.

관측값(observed value)
* 측정값과 비슷한 의미로 쓰이며, 육안이나 기계로 자연 현상 특히 천체나 기상의 상태, 추이, 변화 따위를 관찰하여 측정한 실측값이나 양을 가리킨다.
* 항상 오차를 포함하고 있으므로 관측값에 대한 품질 평가를 하여 신뢰성을 검증하여야 한다.

분산(variance)
* 관측값에서 평균을 뺀 값을 제곱하고, 그것을 모두 더한 후 전체 개수로 나눠서 구한다.
* 차이값의 제곱의 평균이다. 

정규분포
* 평균과 표준편차가 주어져 있을 때 엔트로피를 최대화하는 분포이다.
* 중앙치에 사례 수가 모여있고, 양극단으로 갈수록 X축에 무한히 접근하지만 X축에 닿지는 않는다.
* 좌우 대칭이며 하나의 꼭지를 가진다.

결측치(missing feature)
* 표기되지 않은 값

추세선
* 주가에는 일정한 흐름이 있습니다. 이러한 흐름을 추세라고 하고, 이것을 선으로 표시한 것을 추세선이라고 합니다.
* 상승추세선과 하락추세선 같은 예측할 수 있는 지표 (앞으로 상승할 것이다, 하락할 것이다)
EDA (탐색적데이터분석) Exploratory Data Analysis 
* 데이터 사이언티스트가 데이터세트를 분석하고 조사하여 주요 특성을 파악하는 데에 사용되며, 데이터 시각화 방법을 사용하기도 합니다.

중복값 (Duplicate rows)
* unique 한 'key' 값을 관리해야 하는 경우 중복(duplicates)이 발생하면 분석에 심각한 영향을 끼칠 수도 있습니다.

distinct values = > 중복을 제외한 유일 값 #Pandas 에서는 unique 값
* 유일값 음.. (학번, 주민등록번호 같은 고유 값)

변동계수 (coefficient of variation (CV),상대 표준 편차)
* 표준 편차를 산술 평균으로 나눈 것이다.
* 범위나 분산과 같은 산포도를 계산하는 것만으로는 충분하지 않아 상대적인 산포도를 비교해야 한다.

첨도 (kurtosis)
* 확률분포의 꼬리가 두꺼운 정도를 나타내는 척도이다.
* 얼마나 뾰족한가.
* 첨도값(K)이 3에 가까우면 산포도가 정규분포에 가깝다. 3보다 작을 경우에는(K<3) 산포는 정규분포보다 꼬리가 얇은 분포로 생각할 수 있다, 첨도값이 3보다 큰 양수이면(K>3) 정규분포보다 꼬리가 두꺼운 분포로 판단할 수 있다.

correlation : 상관계수, 상관관계 (통계학에서 상관계수란?) 
	데이터에서 1에 상응한다면 그것은 자기상관
* 두 변수 사이의 통계적 관계를 표현하기 위해 특정한 상관 관계의 정도를 수치적으로 나타낸 계수이다.
* 여러 유형의 상관계수가 존재하지만 제각기 자신들만의 정의와 특징이 있다. 이들은 모두 값의 범위가 -1에서 +1 사이에 속하며 여기서 ±1은 정도가 가장 센 잠재적 일치를 나타내고 0은 정도가 가장 센 불일치를 나타낸다

파이썬라이브러리 단어
hue
* 만약 카테고리형 데이터가 섞여 있는 경우에는 hue 인수에 카테고리 변수 이름을 지정하여 카테고리 값에 따라 색상을 다르게 할 수 있다.

디버깅
* 프로그래밍에서 잘못된 부분을 찾아 고치는 것.


추상화된 도구 라는 궁극적인 의미?
 : 추상화된 도구가 EDA를 훌륭하게 해줌에도 불구하고 판다스로 데이터 분석을 배우는 이유가 무엇인가요?
matplotlib랑 seaborn이 호환이 되는 이유는?
 => seaborn 은 matplolib 을 추상화한 도구

plot :
도표를 만들다[그리다]
corr :
 correlation :상관관계

