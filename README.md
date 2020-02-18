# play-audio


## 添加 Multimedia 模块



  import QtQuick 2.12
  import QtQuick.Controls 2.0
  import QtQuick.Window 2.12
  import QtMultimedia 5.0
  Window {
      visible: true
      width: 640
      height: 480
      title: qsTr("Hello World")

      Audio{
          id:audio
          source:"qrc:/media/busy.mp3"
      }

      Button{
          text :"播放"
          onClicked: {
              audio.play()
          }
      }
  }
