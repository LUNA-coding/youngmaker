---
layout: post
title: "[Luminous] 모식도와 구체적인 기술 설계"
---

전체적인 기기의 틀을 잡았으니, 다음은 구체적인 설계를 시작하였습니다. 논의된 내용은 다음과 같습니다. 라즈베리파이와 연결된 라즈베리파이 카메라에서 사용자의 눈의 영상을 라즈베리파이로 보내주면, 라즈베리파이는 그 데이터를 가지고 인공지능을 사용하여 눈을 감았는지를 판단하고 보드에 연결된 Serial port로 아두이노에게 책을 넘기라는 명령을 보내줍니다.

아두이노가 책을 넘기라는 명령을 받으면, 총 5개의 모터를 사용하여 책을 넘겨주는 작업을 수행하게 됩니다. 모터는 작고 제어가 쉬운 서보 모터를 사용하였고, 부품을 알아보던 중, 아두이노보다 작아 설계에 용이한 LOLIN board라는 아두이노 호환보드를 대신 사용하기로 결정하였습니다.
