# ESPEasy
Easy MultiSensor device based on ESP8266 https://github.com/letscontrolit/ESPEasy

# How To
- [Tutorial Arduino Firmware Upload](https://www.letscontrolit.com/wiki/index.php/Tutorial_Arduino_Firmware_Upload)

# �޸�����

## ����
- ���Ӵ��ؼ�ȩ������ `WZ-S` ֧�� [Plugin 200: Dart WZ-S](ESPEasy/_P200_WZ_S.ino)
- ��������PM2.5+��ȩ+��ʪ�ȴ����� `PMS5003ST` ֧�� [Plugin 201: Plantower PMS5003ST](ESPEasy/_P201_PMS5003ST.ino)

## ������
- ���� `�ٶ� IOT MQTT` ֧�� [Baidu MQTT](ESPEasy/_C014.ino) , ������μ� [�칤-����������](https://cloud.baidu.com/solution/iot/index.html)

## ϵͳ
- �����������ƴ�С��26��Ϊ64����Ϊ�ٶ�MQTT���û����Ƚϳ�����[����ύ](https://github.com/hetaoos/ESPEasy/commit/5d6178165ccef5dd0e6dd6114f4d0c9afca12209)
- MQTT ����֧������ `Client Id`����Ϊ�ٶ�MQTTҪ��`Client Id` �Ƚ����⣬�Զ����ɵ���Ч���߲��������á�[����ύ](https://github.com/hetaoos/ESPEasy/commit/14c33edc02204bbb59d0edb48d6d31b536ce2c5a)
- ��Ĭ���豸�������`DEVICES_MAX`��50��Ϊ60 [����ύ](https://github.com/hetaoos/ESPEasy/commit/f48a1eb1c84332f0378afc349824736c7b2c6dc1)
- ��Ĭ��ÿ�������������������`VARS_PER_TASK`��4��Ϊ8 [����ύ](https://github.com/hetaoos/ESPEasy/commit/f48a1eb1c84332f0378afc349824736c7b2c6dc1)
- ���Ӵ���������`SENSOR_TYPE_*`��Ҳ���Ǳ����������ж��ٸ�������ݵĶ��壺`SENSOR_TYPE_PENTA`��`SENSOR_TYPE_HEXA`�� `SENSOR_TYPE_HEPTA`��`SENSOR_TYPE_OCTA`[����ύ](https://github.com/hetaoos/ESPEasy/commit/f48a1eb1c84332f0378afc349824736c7b2c6dc1)


# ��α���Դ��

## ���ñ��뻷��
PS����Ҫ�Ƕ�[Tutorial Arduino Firmware Upload](https://www.letscontrolit.com/wiki/index.php/Tutorial_Arduino_Firmware_Upload)�ļ�Ҫ˵��
- ���غͰ�װ [`Arduino IDE`](https://www.arduino.cc/en/Main/Software?setlang=cn)
- `�ļ�`-`��ѡ��` �У��޹�`���ӿ������������ַ` Ϊ `http://arduino.esp8266.com/stable/package_esp8266com_index.json`
- `����`-`������"xxxx"`-`�����������` �У����� **ESP8266** ��ѡ��**esp8266 by ESP8266 Community**����ѡ�����°�װ��
- `����`-`������"xxxx"` �У�ѡ��**NodeMCU 1.0 (ESP-12E) Module**
- `����`-`�˿�"xxxx"` �У�Ѱ�ҽ���NodeMCU��ʶ��Ĵ��ڡ�

## ����Դ��
- ���ػ��� clone Դ�뵽����
- �� `Libraries` Ŀ¼�µ�ȫ���ļ������� `�ĵ�\Arduino\Libraries`Ŀ¼��
- ˫���� [`ESPEasy\ESPEasy.ino`](ESPEasy/ESPEasy.ino) ���ɴ� `Arduino IDE`
- �������Դ��󣬵��`��Ŀ`-`�ϴ�`�����ɱ���̼������͵���������

## �����Զ������ã���ѡ��
- ������Ŀ¼�µ� [`Custom-sample.h`](ESPEasy/Custom-sample.h) ���Ʋ�����Ϊ `Custom.h`
- �� `%UserProfile%\AppData\Local\Arduino15\packages\esp8266\hardware\esp8266\2.4.1\platform.txt` �ļ�
  - �ҵ� `build.extra_flags` ����
  - �ں�����Ӳ��� ` -DUSE_CUSTOM_H`
  - ע�⣺·�������ݰ汾��ͬ������Щ��仯
