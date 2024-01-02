#AIT　内田研　2023年度　ROSプログラム

#2024/1/2 途中

##構造
src
  |-devel
    |-record_pub.py
    |-enter_voice_word.txt
    |-sub_face_movie.py
    |-sub_gpt.py
    |-sub_motor.py
  |-package.xml
  |-setup.py
  |-setup.cfg

##ros構造
record_pub→enter_voice_word.txtに保存
  |
  |
sub_gpt
  |-----------
  |           |
sub_face    sub_motor

##各役割
#record_pub
1.音声入力
2.入力音声を音声ファイルに保存
3.入力された音声をテキストファイル変換 
4.Whisper APIを用いて音声ファイル→テキストファイル化

#sub_gpt
