## 안녕하세요! 👋
- 저는 크렘티(Crem2y)입니다.
- FW 엔지니어이고, HW는 취미 레벨로 하는 정도입니다.

## 관심사 💡
- MCU FW
- HW (PCB artwork, schematics, etc.)
- Linux

## 경험 ✈️
### 사용해본 것들
- 언어
  - C, C++
  - Python
  - Lua
  - 등등..
- MCU
  - ARM Cortex-M
    - RP2040, RP2350
    - STM32 (F0, F1, F4)
    - nRF52
  - Other Core
    - ATmega (AVR)
    - ESP32 (RISC-V)
- 통신
  - RS-232, RS-485
  - BLE
  - Ethernet
- HW 설계 툴
  - EasyEDA
  - Altium
  - PADS
- 기타 툴
  - WireShark
  - Docker

## TMI 💤
### 가장 좋아하는 코드
- 고속 역 제곱근. 표준을 다른 방법으로 이용하는 느낌이라 좋아해요
```c
float Q_rsqrt( float number )
{
	long i;
	float x2, y;
	const float threehalfs = 1.5F;

	x2 = number * 0.5F;
	y = number;
	i = * ( long * ) &y;                     // evil floating point bit level hacking
	i = 0x5f3759df - ( i >> 1 );             // what the fuck?
	y = * ( float * ) &i;
	y = y * ( threehalfs - ( x2 * y * y ) ); // 1st iteration
//	y = y * ( threehalfs - ( x2 * y * y ) ); // 2nd iteration, this can be removed

	return y;
}
```


<!--
**Crem2y/Crem2y** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
