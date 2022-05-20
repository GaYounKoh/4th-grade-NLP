# 4th-grade-NLP
NLP <br>
<br>

ref. 사이토코키 밑바닥부터 시작하는 딥러닝 <br>
<br>

[NLP 자연어처리, 한국어 전처리를 위한 기법들](https://ebbnflow.tistory.com/246) <br>
<br>

# 1강
./common/util.py <br>
<br>

# 2강
./ch02/ppmi.py <br>
./ch02/count_method_small.py <br>
./ch02/show_ptb.py <br>
./ch02/count_method_big.py <br>
<br>

# 3강
./common/layers.py <br>
./ch03/cbow_predict.py <br>
>> Matmul class (Affine층과 달리 bias 벡터 없음.)

./ch03/simple_cbow.py <br>
<br>
./common/trainer.py <br>
./ch03/train.py <br>
./common/util.py <br>
<br>
./ch03/simple_skip_gram.py <br>
./common/layers.py <br>
./ch03/train.py <br>
<br>

# 4강
./common/layers.py <br>
./ch04/negative_sampling_layer.py <br>
<br>

# 5강
./common/layers.py <br>
./common/functions.py <br>
./ch04/negative_sampling_layer.py <br>
<br>

# 8강 (220506)
* RNN은 다음 단어 예측하는 도구 <br>
<br>

# 9강
9-10강 어려움. <br>
<br>

# 10강 (220520)
lstm의 혁신적인 점 <br>
잊어버리는 장치를 달았다. <br>
니체의 잠언: 망각은 진전을 낳는다. <br>
그동안엔 정보를 추가할 생각만 했는데 잊어버릴 생각을 하게 된 게 lstm <br>

그렇다고 잊기만 하면 안되니까 추가하는 input gate를 가짐.
input gate는 정보를 선별 (가치있는 정보들만 집어넣음.)