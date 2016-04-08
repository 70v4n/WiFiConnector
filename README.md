[![Build Status](https://travis-ci.org/cmmakerclub/WiFiConnector.svg?branch=master)](https://travis-ci.org/cmmakerclub/WiFiConnector)

# WiFiConnector

WiFi Connector เป็น Arduino Library สำหรับ ESP8266 ที่ถูกสร้างขึ้นมาให้ช่วยให้การต่อ WiFi ง่ายขึ้น และลดความซับซ้อนของโปรแกรมลงไปเพราะว่า การทำงานเป็นแบบเรียก callback เมื่อเกิด Event ต่างๆ

## Events

 - `on_connecting`
 - `on_connected`
 - `on_disconnected`				
 - `on_smartconfig_done`
 - `on_smartconfig_waiting`
 - `on_smartconfig_processing`

## ความสามารถ

 - auto connect เมื่อ Router หรือ wifi ดับไป โดยจะทำงานที่ on_disconnected  และ on_connecting ตามลำดับ
 - รองรับ smartconfig โดยจะเข้าสู่ `on_smartconfig_waiting`, `on_smartconfig_processing`, `on_smartconfig_done` ตามลำดับ

## การเข้าโหมด smart config

 - ในกดปุ่ม flash หรือ GPIO 0 หรือ GPIO ที่ตั้งค่าค้างไว้เป็นเวลา 2 วินาที ในจังหวะที่กำลังงตอนต่อ WiFi เท่านั้น หากกดหลังต่อ WiFi สำเร็จแล้วจะไม่เกิดผลใดๆ

## ตัวอย่างการใช้งาน

[examples/wifi-full-options-config](https://github.com/cmmakerclub/WiFiConnector/tree/master/examples/wifi-full-options-config)

## อ่านบันเรื่องราว อัพเดต และอ่านเพิ่มเติม

[![Join the chat at https://gitter.im/cmmakerclub/WiFiConnector](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/cmmakerclub/WiFiConnector?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
