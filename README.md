# RFID-Attendance-management-program
Attendance management program with pi/ mfrc522


1. 해당 코드는 ChatGPT를 통해 생성되었고 라이선스 규칙에 따라 코드 전부를 공개함.

2. 말 그대로 동작하는 것까지만 확인

3. 라이브러리 코드 저작권 검토는 챗지피티에게 맡겼음. 만약 문제가 되는 부분이 생긴다면 바로 필요한 조치를 취할 수 있도록 문의를 부탁함.

4. 아래는 사용된 라이브러리와 그 라이선스에 관한 개략적인 검토 내용임. 상용화의 경우는 진지하게 생각하지는 않았으나 기회가 생긴 김에 물어봤음.


사용된 라이브러리와 라이센스
아래는 코드에서 사용된 주요 라이브러리와 그 라이센스 정보입니다:

os, time, subprocess, calendar, csv, datetime (Python 표준 라이브러리)

라이센스: Python Software Foundation License (PSFL)
요약: Python의 표준 라이브러리는 자유롭게 사용 및 배포 가능하며, 상업적 사용에도 제한이 없습니다.
RPi.GPIO (라즈베리파이 GPIO 제어 라이브러리)

라이센스: GNU Lesser General Public License (LGPL) v3
요약: 자유로운 사용 및 상업적 배포 가능. 단, 이 라이브러리를 수정하거나 포함할 경우 LGPL 조건에 따라 소스 코드 공개 필요.
mfrc522 (RFID 라이브러리)

라이센스: MIT License
요약: 자유로운 사용, 수정, 배포, 상업적 사용 가능. 소스 코드 공개 의무 없음.
ntplib (NTP 시간 동기화 라이브러리)

라이센스: MIT License
요약: 자유로운 사용, 수정, 배포, 상업적 사용 가능. 소스 코드 공개 의무 없음.
smbus (I2C 통신 라이브러리)

라이센스: GNU General Public License (GPL) v2
요약: 수정된 코드나 이 라이브러리를 포함한 소프트웨어를 배포할 경우 GPL에 따라 소스 코드 공개 필요.
sqlite3 (SQLite 데이터베이스)

라이센스: Public Domain
요약: 자유로운 사용, 수정, 배포 및 상업적 사용 가능. 제약 없음.
matplotlib (데이터 시각화 라이브러리)

라이센스: Matplotlib License (BSD 스타일 라이센스)
요약: 자유로운 사용, 수정, 배포 및 상업적 사용 가능. 제약 없음.
pandas (데이터 분석 라이브러리)

라이센스: BSD 3-Clause License
요약: 자유로운 사용, 수정, 배포 및 상업적 사용 가능. 제약 없음.
라이센스 간 상충 여부
LGPL v3 (RPi.GPIO):

LGPL은 라이브러리를 수정하지 않고 링크만 하는 경우 소스 공개 의무가 없습니다.
코드가 RPi.GPIO를 단순히 호출하는 형태라면, 코드 자체는 LGPL 의무에서 자유롭습니다.
GPL v2 (smbus):

GPL 라이브러리를 사용하는 소프트웨어를 배포할 경우, 소스 코드를 공개해야 합니다.
smbus는 I2C 통신 라이브러리로 사용되었으며, 이로 인해 코드 공개 의무가 발생합니다.
다른 라이브러리들:

MIT, BSD, PSFL 등은 상업적 사용과 배포에 제한이 없으며 GPL 및 LGPL과 충돌하지 않습니다.
무료 배포 / 상용화 / 코드 공개 가능 여부
무료 배포:

가능. 단, smbus(GPL) 사용으로 인해 코드와 관련된 소스 전체를 GPL에 따라 공개해야 합니다.
상용화:

가능. 하지만 상업적 소프트웨어 배포 시 smbus 사용으로 인해 전체 소스 코드를 공개해야 하므로 상용 소프트웨어로 적합하지 않을 수 있습니다.
LGPL(LPI.GPIO) 사용은 상용화에 문제되지 않지만, 수정한 경우 소스 공개 의무가 있습니다.
코드 공개:

가능. GPL 및 LGPL 요구사항에 따라 코드 공개 의무를 준수하면 됩니다.

