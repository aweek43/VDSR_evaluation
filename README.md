# VDSR_evaluation
* 기본 코드는 https://github.com/twtygqyy/pytorch-vdsr 을 참고했습니다
* 채널, 레이어를 바꿔가며 성능을 테스트했습니다.
***
* 성능 지표는 PSNR입니다.
* 위에서부터 성능이 좋은 순입니다.
* x4, x3은 upscale factor(확대 계수) 입니다.
* 분석: bicubic과 비교했을 때 사실 차이가 거의 없었다.
* 채널, 레이어를 바꿔도 아주 미세한차이만 있을 뿐 의미있는 차이를 만들어 내지 못하였다.
* 이는 사용한 데이터셋(Set 5)가 너무 작고 충분한 epoch(50)를 주지 못하였기 때문이다.
* 또한 Colab 사용 시 레이어가 깊을 때 오히려 시간이 적게 걸린 경우가 있는데,
* 이는 단순히 colab이 클라우드로 GPU를 쓰기 때문에 사용 당시 트레픽이 영향을 주었을 것으로 분석된다.

* https://blog.naver.com/kimhanju7/221465477915
