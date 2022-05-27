
# FLに関するドキュメント

## FLのライフサイクル
## FedAvg vs FedSGD
### FedSGD
- デバイスから送られたgradientsかパラメータをサーバーに送る
- サーバーで平均かしたgradientsかパラメータを新しいパラメータに適応する
- デバイスとサーバー間であまり通信しない
- FedAvgよりNaive? 

<img width="624" alt="スクリーンショット 2022-05-27 11 15 53" src="https://user-images.githubusercontent.com/61937077/170615319-cf6fe956-7d17-4ac9-af2e-f72177fd2f9e.png">

### FedAvg
<img width="619" alt="スクリーンショット 2022-05-27 11 17 50" src="https://user-images.githubusercontent.com/61937077/170615519-7c427468-44bf-4341-97a5-1fc1efbe753f.png">


### 確率的勾配法
- デバイス自体を反復学習させて、勾配降下法を用いてパラメータを更新する
- デバイスからサーバーにパラメータを送信する
- サーバーは平均化されたパラメータを新しいパラメータと適合する
- FedSGDより通信量が少ない
- 適切なハイパーパラメータを使用すれば、Fedsgdよりも優れたパフォーマンスを発揮することができる



## FLフレームワーク
> https://flower.dev

