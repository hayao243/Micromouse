【仕様】
・シリアルコンソールの入力内容（1文字＆割り込み）に応じて動作変更

mode_move用
Z：停止
W：前進
A：左回転
S：後退
D：右回転

mode_display用
1：センサ情報の表示
2：姿勢（9軸センサ）の情報表示

・シリアルにかかわらず実行する
タイマー割り込みで、姿勢とセンサー距離の取得
青ボタンを押したらPWM停止


【ピン】
・UART2
TX：PA2
RX：PA3

・UART1
TX： PB6
RX： PB7 

・PWM
左タイヤ
前進　TIM2_CH1：PA5
後進    TIM3_CH1：PA6
右タイヤ
前進    TIM1_CH1：PA8
後進    TIM5_CH2：PA1

・青ボタン
PC13　

・距離センサ
トリガー　GPIO Output：PC4
エコー　    GPIO EXTI5：PC5

・9軸センサ
SCL：PB8
SDA：PB9

・割り込み用タイマー　
TIM11
