---
layout: line_tracer
title: Line-Tracer
permalink: /line-tracer/
---

각 로봇의 스펙이나 자세한 내용은 위 링크를 참조

## 라인 트레이서란?

라인트레이서는 검정색 바탕의 경기장에 그려진 흰색 라인을 따라서 움직이는 마이크로 로봇이다.   
출발 지점부터 종료 지점까지의 폐곡선 내의 주행한 기록을 단축시키는 것을 목표로 한다.   
라인트레이서는 다음과 같은 세 부분으로 구성한다.
    
- 로봇의 위치와 라인의 형태를 판별하는 센서부   
- 센서에서 수집된 데이터를 분석하여 제어 명령을 내리는 제어부   
- 제어 명령을 수행하여 로봇의 이동을 담당하는 구동부

주어진 시간 또는 제한된 주행 횟수 내에 가장 빠르게 주행하여 기록을 받아야 한다.   
보통 주행은 탐색 주행과 가속 주행으로 나누어진다.

## 제작 목적

1. 로봇 제작을 처음 시작할 때 추천되는 로봇인 라인 트레이서는 다른 로봇에 비해 접근이 쉽다.   
2. 빠르게 주행하려 할수록 역학, 제어, 미적분 등 다양한 분야의 지식을 필요로 하며, 최단 패스를 좇는 알고리즘에 따라 로봇의 성능 차이가 심하게 나타난다.
3. 학과 전공시간에 배운 지식을 라인 트레이서에 적용시켜 실제 사용되는 방법과 이론을 습득하는 것으로 목적으로 한다.

## 개발 기간

Gara(가라) : 2020년 1월 ~ 2022년 9월   
CAM(캠) : 2022년 7월 ~ 2022년 9월

## 사용 소프트웨어

1. Source Insight
2. Solid Works
3. Matlab

## 사용된 이론 및 기술

### 라인 트레이서 공통

1. Using DSP(TMS320F2809) / GPIO, ADC, PWM, Interrupt
2. Sliding Window Algorithm 

### [Gara: Stepper Motor Line Follower](https://nodang.github.io/line-tracer/Gara/) 

1. Using C Language
2. 2-Phase Stepper Motor Control / Full-Step Drive
3. Motion Control of Vehicle using **Jerk** and Simulation using Matlab

### [CAM: Line Follower Using Raspberry Pi](https://nodang.github.io/line-tracer/CAM/)

1. Using Python3, OpenCV2 for Image Processing
1. SCI(Serial Communication Interface) Between DSP and Raspberry PI

## 시연 영상

아래는 2022년도 단국대 대회에 출전한 스텝트레이서(가라)의 영상이다.

<div class="respondFrame">
  <iframe src="https://www.youtube.com/embed/8kcgrF84E4c?start=114" frameborder="0" allowfullscreen></iframe>
</div>