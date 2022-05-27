# 4th-grade-NLP
NLP <br>
<br>

ref. 사이토코키 밑바닥부터 시작하는 딥러닝 <br>
<br>

[NLP 자연어처리, 한국어 전처리를 위한 기법들](https://ebbnflow.tistory.com/246) <br>
<br>

# 참고 페이지
[파이썬 용어정리;  라이브러리 >= 패키지 >= 모듈 > 클래스 > 메소드 = 함수;;; 객체...](https://pybasall.tistory.com/147) <br>


* 라이브러리 >= 패키지 >= 모듈 > 클래스 > 메소드 = 함수;;; 객체..

* 라이브러리: 패키지 혹은 패키지를 모아놓은 것
* 패키지: 모듈 혹은 모듈을 모아놓은 것
* 모듈: 함수, 변수, 클래스를 모아놓은 것
* 
* 클래스: 속성과 함수를 포함하는 구조
* 메소드: 클래스 안에 정의된 함수
* 함수: 입력값을 받고 지정한 연산을 수행하여 결과값을 출력
* 객체: 속성과 메소드를 가진 모든 것


<br>

[함수, 메소드, 모듈, 내장함수, 내장모듈의 의미와 차이](https://blog.naver.com/youndok/222032150902) <br>

> ## 함수

* 람다함수: 함수 이름이 없는 1회용, 한 줄에 정의하여 사용하는 함수 <br>

람다함수 예제
``` python
user_fn = lambda x, y : x + y
sum = user_fn(10,6)
```

* 메소드: 특정 객체 (object)에 적용되는 함수 <br>

메소드 예시
``` python
str.replace()
str.count()
str.split()
list.append()
tuple.index()
# ...
```

> ## 모듈
* 모듈: python 명령어로 이루어진 python 프로그램 파일 (확장자 .py) <br>

<모듈 예시>
``` python
import user_python_file
sum = user_python_file.user_fn(10,6)
```
[user_python_file.py] 안에는 다음과 같은 함수가 정의돼 있음.
``` python
def user_fn(x,y):
    return x+y
```

* 내장모듈: python 언어 자체에 통합되어 제공되는, C언어로 작성된 모듈 <br>

내장모듈 예시
``` python
import os
os.mkdir('directory')
```
<br>

[패키지, 모듈, 함수, 메소드 용어정리](https://data-rider.blogspot.com/2015/11/blog-post_17.html) <br>

[내장 dir()함수 이용해 객체가 가지고있는 메소드 찾기](http://daplus.net/python-%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EA%B0%9D%EC%B2%B4%EA%B0%80-%EA%B0%80%EC%A7%80%EA%B3%A0%EC%9E%88%EB%8A%94-%EB%A9%94%EC%86%8C%EB%93%9C-%EC%B0%BE%EA%B8%B0/) <br>
[dir() 이해하기](https://www.delftstack.com/ko/howto/python/python-list-functions-in-module/) <br>
<br>


# 1강 시소러스와 동시발생행렬
./common/util.py <br>
<br>

# 2강 동시발생행렬 개선 (정보이론과 SVD)
./ch02/ppmi.py <br>
./ch02/count_method_small.py <br>
./ch02/show_ptb.py <br>
./ch02/count_method_big.py <br>
<br>

# 3강 word2vec 프로토타입
./common/layers.py <br>
./ch03/cbow_predict.py <br>
>> Matmul class (Affine층과 달리 bias 벡터 없음.)

./ch03/simple_cbow.py <br>
--- <br>
./common/trainer.py <br>
./ch03/train.py <br>
./common/util.py <br>
--- <br>
./ch03/simple_skip_gram.py <br>
./common/layers.py <br>
./ch03/train.py <br>
<br>

# 4강 embedding 층과 embedding dot층
./common/layers.py <br>
./ch04/negative_sampling_layer.py <br>
<br>

# 5강 sigmoid with loss층과 negative sampling
./common/layers.py <br>
./common/functions.py <br>
./ch04/negative_sampling_layer.py <br>
<br>

# 6강 king - man + woman = queen
./ch04/cbow.py <br>
./ch04/train.py <br>
./common/trainer.py <br>
./ch04/eval.py <br>
./common/util.py <br>
./ch04/skip_gram.py <br>
<br>

# 🔺🔺----------- 중간 ------------🔺🔺 #

# 🔻🔻----------- 기말 ------------🔻🔻 #

# 7강 순환신경망과 언어모델
./common/time_layers.py ~ RNN class <br>
<br>

# 8강 RNN층의 시간에 대한 역전파 (220506)
* RNN은 다음 단어 예측하는 도구 <br>

./common/time_layers.py ~ TimeRNN class <br>
<br>

# 9강 RNN 언어모델의 구현과 학습
* 9-10강 어려움. <br>

./common/time_layers.py ~ TimeEmbedding class, TimeAffine class, TimeSoftmaxWithLoss class <br>
./ch05/simple_rnnlm.py <br>
./ch05/train_custom_loop.py <br>
train custom loop data.py <br>
./ch05/train.py <br>
./trainer.py <br>
<br>

# 10강 LSTM (220520)
* *lstm의 혁신적인 점 <br>
잊어버리는 장치를 달았다. <br>

./ch06/rnn_gradient_graph.py <br>
./ch06/clip_grads.py <br>
./common/time_layers.py ~ LSTM class TimeLSTM class <br>
<br>

## 니체의 잠언: <span style = 'color:red'> **망각은 진전을 낳는다.** </span> <br>
<br>

그동안엔 정보를 추가할 생각만 했는데 잊어버릴 생각을 하게 된 게 lstm <br>
<br>

그렇다고 잊기만 하면 안되니까 추가하는 input gate를 가짐. <br>
<span style = 'color:red'> <font size = 4> ***input gate***</font></span>는 정보를 선별 (가치있는 정보들만 집어넣음.) <br>


적절히 잊어버리고 적절히 추가
그 <span style = 'color:red'>**'적절히'**</span>의 밸브는 weight와 bias가 조절 <br>
<br>


# 11강 RNN 언어모델의 개선 (LSTM, multi-layer, drop-out, weight tying) (220527)
./ch06/rnnlm.py <br>
./ch06/train_rnnlm.py <br>
./ch06/eval.py ~ model을 Rnnlm()로<br>
./common/base_model.py <br>
--- <br>
./ch06/better_rnnlm.py <br>
./ch06/train_better_rnnlm.py <br>
./common/time_layers.py ~ TimeDropout class <br>
./ch06/eval.py ~ model을 BetterRnnlm()으로 바꾸기 <br>
<br>

drop out: 랜덤하게 끊는 것. <br>
세로로? 가로로? <br>

해보니 그렇더라~ 딥러닝의 오류엔 명확한 이유 없는 경우도 있음. <br>

파라미터가 많은게 오버피팅을 야기할 수도 있음. <br>

딥러닝은 항상 적당히 잘 <br>

drop out은 test할 때는 죽이지 않음 (죽이진 않고 사이즈 재조정) <br>

녹강에서 설명안한 reset state (2번 문제와 3번 문제 사이에 hidden, cell state 초기화를 해줘야 함.) <br>

층을 깊게 쌓으면 문제가 발생함. <br>
<br>

# 12강 문장 생성 (실강 없음.)
./ch07/rnnlm_gen.py <br>
./ch06/rnnlm.py <br>
./ch07/generate_text.py <br>
./ch06/train_better_rnnlm.py <br>
./ch07/generate_better_test.py <br>
./common/time_layers.py <br>

# 13강 seq2seq (기계번역과 챗봇의 원리) (실강 없음.)
./ch07/seq2seq.py <br>

