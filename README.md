https://youtu.be/1ElgyAAYoH4  
シューティングゲームのYouTubeアドレス

![1](https://user-images.githubusercontent.com/55978194/98229051-c5462580-1f9c-11eb-8607-17c1b9019367.png)
![2](https://user-images.githubusercontent.com/55978194/98229519-59b08800-1f9d-11eb-9c11-043d6c2ebed8.png)

Project information
=============
## Requirement
1. PyGame
2. anaconda
3. tensorflow
4. numpy

Environment
=============
![1](https://user-images.githubusercontent.com/55978194/84865962-0b652000-b0b4-11ea-94d9-1e5f6f18d941.png)
1. 10×10配列を作った後、この配列でパイゲームを使って視覚的に制作
2. 0は Map 1は Agent 2は Enemy

Agent
=============
![sprite1](https://user-images.githubusercontent.com/55978194/84870916-dc05e180-b0ba-11ea-8329-0762be789882.png)
1. Environmentと相互作用をしながら上下二つのActionを選択
2. Actionを選択後、EnemyとぶつからなければRewardを1獲得
3. もしEnemyとぶつかったら Rewardを-30させてから Reset

Enemy 
=============
![enemy1](https://user-images.githubusercontent.com/55978194/84871944-26d42900-b0bc-11ea-9339-ce9ddcd60064.png)
1. Enviromentでは2に表現され、1に表現されるAgentとぶつかったらRewardを-30させてからReset

State, Step
=============
![me](https://user-images.githubusercontent.com/55978194/84872705-3011c580-b0bd-11ea-8f35-6fe8cbefac4c.png) ![you](https://user-images.githubusercontent.com/55978194/84873052-9bf42e00-b0bd-11ea-8ce1-c7dca765a945.png)
1. MySpriteクラスで臨時環境(board上のAgentの位置を表示)を作り出す。
2. EnemyクラスでMySpriteで作り出した臨時環境を使って完璧なNextState{board上のAgent(1)とEnemy(2)}を作り出す。
![temp](https://user-images.githubusercontent.com/55978194/84873200-dc53ac00-b0bd-11ea-98bf-feed537a8dcb.png)

Deep Q network
=============
![ss](https://user-images.githubusercontent.com/55978194/84881793-50e01800-b0c9-11ea-9d72-e6ba3aa60383.png)
1. ネットワークを構成後、Predict、Update関数生成

Replay Memory
=============
1. Agentをすぐに学習させずに一定量を保存しておいて一度に学習。

Target, Main network
=============
1. Target networkとMainnetworkを分離して学習した後、コピー

Step count
=============
![s](https://user-images.githubusercontent.com/55978194/84881456-d7482a00-b0c8-11ea-8d77-62337c35ff88.png)
1. AgentがStepを300以上したらPyGameで画面に出力
2. Stepが600以上ならゲーム開始











YouTube Address of Self-driving Video



自動走行技術映像
https://youtu.be/LP_2BtZ9CH0
![2](https://user-images.githubusercontent.com/55978194/84866198-567f3300-b0b4-11ea-80e7-5554df0d0e06.png)





自動走行映像
https://youtu.be/7mZ08CRm0IA
![1](https://user-images.githubusercontent.com/55978194/84866440-b1b12580-b0b4-11ea-97a2-c3d2a689c2c1.png)
