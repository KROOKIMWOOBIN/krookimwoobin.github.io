---
title: "PriorityQueue"
excerpt: "완전 이진 트리"

categories: [Algorithm]
tags: [Algorithm, Java]

toc: true
toc_sticky: true

date: 2024-05-02 15:03:00 +0800
last_modified_at: 2024-04-27 14:00:00 +0800

pin: false
---

## PriorityQueue란?
>일반적인 큐는 먼저 들어간 데이터가 먼저 나가는 구조인(FIFO) 형식의 자료구조입니다.
반면에 우선순위 큐의 경우 순서와는 상관없이 우선순위가 높은 데이터가 
먼저 나가는 자료구조입니다.

## PriorityQueue 선언 방법
```Java
// 우선순위가 낮은 숫자가 먼저 나옴(작은 숫자)
PriorityQueue<T> pQ = new PriorityQueue<>();
// 우선순위가 높은 숫자가 먼저 나옴(큰 숫자)
PriorityQueue<T> pQ = new PriorityQueue<>(Collections.reverseOrder());
```

## 기본적인 메소드

### 삽입
1. pQ.add(value);
   - 반환 값 : 삽입 성공 시 true / 실패 시 Exception 발생
2. pQ.offer(value);
   - 반환 값 : 삽입 성공 시 true / 실패 시 false 반환 

### 삭제
1. pQ.remove();
   - 반환 값 : 삭제된 value / 공백 큐이면 Exception 발생
2. pQ.remove(value);
   - 반환 값 : 해당 값이 존재하면 해당 값 삭제 후 true / 없으면 false 반환 
3. pQ.poll();
   - 반환 값 : 삭제된 value / 공백 큐이면 null 반환

### HEAD에 값 반환
1. pQ.element();
   - 반환 값 : Head에 위치한 값 / 공백 큐이면 Exception 발생
2. pQ.peek();
   - 반환 값 : Head에 위치한 값 / 공백 큐이면 null 발생

### 초기화
1. pQ.clear();
   - 반환 값 : X

### 크기
1. pQ.size();
   - 반환 값 : 사이즈 반환

### 해당 원소가 존재하는지?
1. pQ.contains(value)
   - 반환 값 : 값이 존재하면 true / 값이 없으면 false 반환

### 공백인가?
1. pQ.isEmpty();
   - 반환 값 : 공백 큐이면 true / 아니면 false 반환 