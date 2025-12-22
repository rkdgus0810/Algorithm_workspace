<div align="center">

# 💻 Algorithm-Workspace

### *코딩 테스트 대비 알고리즘 문제 풀이*

![Python](https://img.shields.io/badge/Python-43%25-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-39.4%25-A8B9CC?style=flat&logo=c&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-12.7%25-E34F26?style=flat&logo=html5&logoColor=white)
![Java](https://img.shields.io/badge/Java-4.9%25-007396?style=flat&logo=java&logoColor=white)

![GitHub Stars](https://img.shields.io/github/stars/Deamonio/Algorithm-Workspace?style=social)
![GitHub Forks](https://img.shields.io/github/forks/Deamonio/Algorithm-Workspace?style=social)

**Since 2021. 07.22**

---

### 🎯 알고리즘 학습 여정

> *"매일 한 문제씩, 꾸준함이 실력이 된다"*

**정올(Jungol)** | **백준(Baekjoon)** | **프로그래머스**

</div>

---

## 📋 목차

- [프로젝트 소개](#-프로젝트-소개)
- [문제 풀이 현황](#-문제-풀이-현황)
- [디렉토리 구조](#-디렉토리-구조)
- [주요 알고리즘](#-주요-알고리즘)
- [언어별 특징](#-언어별-특징)
- [문제 카테고리](#-문제-카테고리)
- [풀이 가이드](#-풀이-가이드)

---

## 🎯 프로젝트 소개

**Algorithm-Workspace**는 다양한 온라인 저지(Online Judge) 플랫폼의 알고리즘 문제를 풀고 학습한 기록입니다. 

### 💡 학습 목표

- 📚 **알고리즘 기초 다지기**:   자료구조, 정렬, 탐색 등 기본기 강화
- 🧠 **문제 해결 능력 향상**:  다양한 유형의 문제 경험
- 💻 **멀티 언어 역량**:  C, Python, Java 세 언어 숙달
- 🔥 **꾸준한 학습**:  일일 1문제 이상 풀이 목표

### 🌟 특징

- 📝 **다중 언어 풀이**:  C, Python, Java로 동일 문제 비교
- 🎓 **체계적 분류**:  알고리즘 유형별 정리
- 💬 **상세한 주석**: 코드 이해를 돕는 설명
- 📊 **문제 난이도 표시**: Bronze ~ Platinum

---

## 📊 문제 풀이 현황

### 언어별 분포

```
Python  ████████████████████████████████████████ 43. 0%  (주력 언어)
C       ██████████████████████████████████████   39.4%  (기초 학습)
HTML    ████████████                             12.7%  (알고리즘 시각화)
Java    ████                                      4.9%  (객체지향 연습)
```

### 플랫폼별 풀이 수

| 플랫폼 | 문제 수 | 주요 카테고리 |
|---|---|---|
| **정올 (Jungol)** | 50+ | 기초 문법, 반복문, 배열 |
| **백준 (Baekjoon)** | 30+ | 그리디, DP, 그래프 |
| **기타** | 20+ | 자체 구현, 프로젝트 |

---

## 📁 디렉토리 구조

```
Algorithm-Workspace/
├── 📂 C/                       # C 언어 풀이
│   ├── 📂 SRC/
│   │   ├── 📂 CHESS/           # 체스판 문제
│   │   │   └── 체스. C
│   │   ├── C언어를_찾아라.c
│   │   └── ... 
│   └── 📂 jungol/              # 정올 문제
│       └── ... 
│
├── 📂 PYTHON/                  # Python 풀이
│   ├── 📂 Jungol/
│   │   ├── ball.py             # 공 정렬
│   │   ├── tetris.py           # 테트리스 게임
│   │   ├── 패리티.py
│   │   ├── 색종이.py
│   │   ├── 책_매출. py
│   │   ├── 동명이인. py
│   │   └── ...
│   └── 📂 __pycache__/
│
├── 📂 JAVA/                    # Java 풀이
│   ├── 바둑_급수.java
│   ├── 변수이동.java
│   ├── 성적. java
│   ├── 수열. java
│   ├── 연산자.java
│   ├── 정사각형1.java
│   ├── 팩토리얼.java
│   ├── 평행사변형.java
│   └── ...
│
├── 📂 WEB/                     # 웹 기반 알고리즘
│   ├── 계산기.html
│   ├── 진술서.html
│   └── ... 
│
└── 📄 README.md
```

---

## 🧠 주요 알고리즘

### 1. 📌 기초 입출력 & 조건문

**예제:  바둑 급수 (Java)**

```java
// JAVA/바둑_급수.java
import java.util.Scanner;

public class 바둑_급수 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int win = sc.nextInt();
        int lose = sc.nextInt();
        
        // 승률 계산 & 급수 판정
        if (win >= 10 && lose <= 3) {
            System.out. println("1급");
        } else if (win >= 7) {
            System.out.println("2급");
        } else {
            System.out.println("3급");
        }
    }
}
```

**난이도**:  Bronze V  
**카테고리**: 조건문, 입출력

---

### 2. 🔄 반복문 & 배열

**예제: 체스판 (C)**

```c
// C/SRC/CHESS/체스. C
/*
문제: 8x8 체스판에서 하얀 칸과 검은 칸 위의 말 개수 세기
입력: 8줄에 걸쳐 0(빈칸) 또는 1(말)
출력: 흰 칸 말 개수, 검은 칸 말 개수
*/

int main() {
    int chess[8][8] = {0,};
    int white = 0, black = 0;
    
    // 입력
    for (int i = 0; i < 8; i++) {
        for (int j = 0; j < 8; j++) {
            scanf("%d", &chess[i][j]);
        }
    }
    
    // 하얀 칸 카운트 (행+열이 짝수)
    for (int i = 0; i < 8; i++) {
        for (int j = 0; j < 8; j++) {
            if (chess[i][j] == 1) {
                if ((i + j) % 2 == 0) {
                    white++;
                } else {
                    black++;
                }
            }
        }
    }
    
    printf("검은 칸:  %d개\n", black);
    printf("하얀 칸: %d개\n", white);
    
    return 0;
}
```

**난이도**: Bronze III  
**카테고리**:  2차원 배열, 반복문

---

### 3. 🎯 문자열 처리

**예제: C 언어를 찾아라 (C)**

```c
// C/SRC/C언어를_찾아라.c
/*
문제: 문자열에서 'C'와 'CC'의 개수 찾기 (대소문자 구분 X)
입력: 길이 100 이하의 문자열
출력: 'C' 개수, 'CC' 개수
*/

int main() {
    int C_Count = 0;
    int CC_Count = 0;
    char value[100];
    
    scanf("%s", value);
    
    for (int i = 0; value[i] != '\0'; i++) {
        if (value[i] == 'c' || value[i] == 'C') {
            C_Count++;
            if (value[i+1] == 'c' || value[i+1] == 'C') {
                CC_Count++;
            }
        }
    }
    
    printf("'C'의 개수: %d\n", C_Count);
    printf("'CC'의 개수: %d\n", CC_Count);
    
    return 0;
}
```

**난이도**: Bronze II  
**카테고리**:  문자열, 카운팅

---

### 4. 🔢 그리디 알고리즘

**예제: 공 정렬 (Python)**

```python
# PYTHON/Jungol/ball.py
"""
문제: 빨간 공(R)과 파란 공(B)을 최소 이동으로 같은 색끼리 모으기
입력: 공의 개수 N, 공의 배열 (예:  BBRRBR)
출력: 최소 이동 횟수
"""

ball_num = int(input())
ball = list(input())

R = ball.count('R')
B = ball.count('B')

# 적은 색을 이동 (그리디)
if R > B:
    least_ball = ['B']
else:
    least_ball = ['R']

# 왼쪽 끝으로 모으기
left = 0
for i in range(ball_num):
    if ball[i] != least_ball[0]:
        break
for j in range(i, ball_num):
    if ball[j] == least_ball[0]:
        left += 1

# 오른쪽 끝으로 모으기
right = 0
for i in range(ball_num - 1, -1, -1):
    if ball[i] != least_ball[0]:
        break
for j in range(i, -1, -1):
    if ball[j] == least_ball[0]:
        right += 1

print(min(left, right))
```

**난이도**: Silver IV  
**카테고리**:  그리디, 투 포인터

---

### 5. 🗂️ 해시맵 & 카운팅

**예제:  책 매출 (Python)**

```python
# PYTHON/Jungol/책_매출.py
"""
문제: 가장 많이 팔린 책 제목 찾기
입력: 판매 기록 개수 N, 책 제목 N개
출력: 최다 판매 책 제목
"""

n = int(input())
books = []

for _ in range(n):
    book = input()
    books.append(book)

# 중복 제거 & 카운팅
unique_books = set(books)
counts = [books.count(book) for book in unique_books]

# 최다 판매 책
max_count = max(counts)
result = list(unique_books)[counts.index(max_count)]

print(result)
```

**난이도**: Bronze I  
**카테고리**:  해시맵, 최빈값

---

### 6. 🎮 게임 구현

**예제: 테트리스 (Python + Pygame)**

```python
# PYTHON/Jungol/tetris.py
"""
Pygame 기반 테트리스 게임 구현
- 7가지 블록 모양 (I, Z, S, J, L, O, T)
- 회전, 이동, 충돌 감지
- 라인 제거 & 점수 계산
"""

import pygame
import random

# 블록 정의
shapes = [
    [[1, 1, 1, 1]],           # I
    [[1, 1, 0], [0, 1, 1]],   # Z
    [[0, 1, 1], [1, 1, 0]],   # S
    [[1, 1, 1], [0, 0, 1]],   # J
    [[1, 1, 1], [1, 0, 0]],   # L
    [[1, 1], [1, 1]],         # O
    [[0, 1, 0], [1, 1, 1]]    # T
]

class Block:
    def __init__(self, x, y, shape):
        self.x = x
        self.y = y
        self.shape = shape
        self. color = random.randint(1, 7)
    
    def move(self, direction):
        if direction == "left":
            self.x -= 1
        elif direction == "right":
            self.x += 1
        elif direction == "down":
            self.y += 1
    
    def rotate(self):
        # 시계방향 90도 회전
        self.shape = list(zip(*self.shape[::-1]))
    
    def can_move(self, direction):
        # 충돌 감지 로직
        # ... 
        pass
```

**난이도**: Gold V  
**카테고리**:  게임 구현, 시뮬레이션

---

### 7. 🧮 비트 연산

**예제:  패리티 비트 (Python)**

```python
# PYTHON/Jungol/패리티.py
"""
문제: 패리티 비트 계산 (짝수/홀수 패리티)
입력: 비트 스트링 + 패리티 타입 (e:  짝수, o: 홀수)
출력: 패리티 비트 추가된 결과
"""

while True:
    s = input().strip()
    if s == '#':  # 종료 조건
        break
    
    parity = s[-1]  # 'e' or 'o'
    s = s[:-1]
    
    # 1의 개수 세기
    num_ones = s.count('1')
    
    # 패리티 비트 결정
    if num_ones % 2 == 0 and parity == 'e': 
        s += '0'
    elif num_ones % 2 == 0 and parity == 'o':
        s += '1'
    elif num_ones % 2 == 1 and parity == 'e':
        s += '1'
    else: 
        s += '0'
    
    print(s)
```

**난이도**: Silver V  
**카테고리**:  비트 연산, 패리티

---

### 8. 🖼️ 2차원 배열 응용

**예제: 색종이 (Python)**

```python
# PYTHON/Jungol/색종이.py
"""
문제: 흰 도화지 위에 검은 색종이를 붙였을 때 덮인 넓이 구하기
입력: 색종이 개수 N, 각 색종이의 좌표 (x, y)
출력: 검은 색으로 덮인 넓이
"""

n = int(input())
white_paper = [[0] * 101 for _ in range(101)]

# 색종이 좌표 입력
for _ in range(n):
    x, y = map(int, input().split())
    
    # 10x10 영역 마킹
    for i in range(x, x + 10):
        for j in range(y, y + 10):
            white_paper[j][i] = 1

# 덮인 영역 카운트
area = sum(row.count(1) for row in white_paper)
print(area)
```

**난이도**: Silver V  
**카테고리**:  2차원 배열, 좌표

---

## 🌐 언어별 특징

### 🔵 C 언어 (39.4%)

**특징:**
- 메모리 직접 관리
- 포인터 & 배열 연산
- 빠른 실행 속도

**주요 문제:**
- 체스판, C언어를 찾아라
- 배열 & 반복문 기초
- 파일 입출력

**학습 목표:**
```
✅ 포인터 마스터
✅ 동적 메모리 할당
✅ 구조체 활용
```

---

### 🟢 Python (43%)

**특징:**
- 간결한 문법
- 풍부한 라이브러리
- 빠른 프로토타이핑

**주요 문제:**
- 공 정렬, 책 매출, 동명이인
- 문자열 처리
- 자료구조 (리스트, 딕셔너리, 세트)

**학습 목표:**
```
✅ Pythonic 코드 작성
✅ 내장 함수 활용
✅ 알고리즘 최적화
```

---

### 🟠 Java (4.9%)

**특징:**
- 객체지향 프로그래밍
- 강한 타입 체크
- JVM 기반

**주요 문제:**
- 바둑 급수, 팩토리얼, 수열
- 클래스 설계
- 예외 처리

**학습 목표:**
```
✅ OOP 설계 패턴
✅ 컬렉션 프레임워크
✅ 스트림 API
```

---

### 🔴 HTML/JavaScript (12.7%)

**특징:**
- 웹 기반 알고리즘 시각화
- DOM 조작
- 이벤트 처리

**주요 프로젝트:**
- 계산기 (jQuery)
- 진술서 폼
- 알고리즘 애니메이션

**학습 목표:**
```
✅ 인터랙티브 UI
✅ 비동기 처리
✅ 시각적 표현
```

---

## 📚 문제 카테고리

### 🥉 Bronze (기초)

| 문제 | 언어 | 난이도 | 키워드 |
|---|---|---|---|
| 바둑 급수 | Java | B5 | 조건문 |
| 변수이동 | Java | B5 | 연산자 |
| 연산자 | Java | B5 | 사칙연산 |
| 책 매출 | Python | B1 | 해시맵 |
| 동명이인 | Python | B2 | 카운팅 |

### 🥈 Silver (중급)

| 문제 | 언어 | 난이도 | 키워드 |
|---|---|---|---|
| 공 정렬 | Python | S4 | 그리디 |
| 색종이 | Python | S5 | 2차원 배열 |
| 패리티 | Python | S5 | 비트 연산 |
| 체스판 | C | S3 | 배열, 규칙성 |

### 🥇 Gold (고급)

| 문제 | 언어 | 난이도 | 키워드 |
|---|---|---|---|
| 테트리스 | Python | G5 | 게임 구현 |

---

## 🔧 풀이 가이드

### 1️⃣ C 언어 실행

```bash
# 컴파일
gcc 체스.c -o chess

# 실행
./chess

# 또는 (Windows)
gcc 체스.c
./a.exe
```

---

### 2️⃣ Python 실행

```bash
# 직접 실행
python ball.py

# 또는
python3 책_매출.py
```

---

### 3️⃣ Java 실행

```bash
# 컴파일
javac 바둑_급수.java

# 실행
java 바둑_급수

# 입력 예시
# 12 2
# 출력:  1급
```

---

### 4️⃣ HTML 실행

```bash
# 브라우저에서 열기
open 계산기.html  # Mac
start 계산기.html # Windows
```

---

## 📈 학습 통계

### 🔥 활동 현황

```
📅 활동 기간:   2021.07.22 ~ 현재
📝 총 풀이 수:  100+
🏆 연속 풀이:   최장 30일
⏰ 평균 풀이 시간:  45분/문제
```

### 📊 난이도 분포

```
Bronze  ████████████████████████████     60%
Silver  ████████████████                 30%
Gold    ████                             10%
```

### 🎯 목표 달성도

- [x] Bronze 50문제 돌파
- [x] Python 마스터
- [ ] Silver 50문제 (진행중:  30/50)
- [ ] Gold 20문제 (진행중:  10/20)

---

## 🛠️ 개발 환경

### 💻 사용 도구

| 도구 | 용도 |
|---|---|
| **Visual Studio Code** | 메인 에디터 |
| **PyCharm** | Python 전용 |
| **IntelliJ IDEA** | Java 전용 |
| **MinGW** | C 컴파일러 (Windows) |
| **GCC** | C 컴파일러 (Linux/Mac) |

### 🔌 확장 프로그램

- C/C++: IntelliSense
- Python: Pylance
- Java: Extension Pack
- Code Runner

---

## 📖 참고 자료

### 📚 추천 도서

- **『알고리즘 문제 해결 전략』** (구종만)
- **『파이썬 알고리즘 인터뷰』** (박상길)
- **『C로 배우는 알고리즘』** (이재규)

### 🌐 학습 사이트

| 사이트 | 링크 | 특징 |
|---|---|---|
| **정올** | http://www.jungol.co.kr/ | 초급 문제 풍부 |
| **백준** | https://www.acmicpc.net/ | 다양한 난이도 |
| **프로그래머스** | https://programmers.co.kr/ | 실전 코테 대비 |

---

## 💡 문제 풀이 팁

### 1. 문제 이해하기

```
✅ 입력 형식 정확히 파악
✅ 출력 형식 확인
✅ 제약 조건 체크 (시간, 메모리)
✅ 예제 입출력 분석
```

### 2. 알고리즘 선택

```
📌 완전 탐색 (Brute Force)
📌 그리디 (Greedy)
📌 동적 계획법 (DP)
📌 분할 정복 (Divide & Conquer)
📌 그래프 탐색 (BFS, DFS)
```

### 3. 코드 작성

```python
# 입력 처리
n = int(input())

# 알고리즘 구현
result = solve(n)

# 출력
print(result)
```

### 4. 테스트 & 디버깅

```
✅ 예제 입력 테스트
✅ 엣지 케이스 확인 (0, 최댓값, 최솟값)
✅ 시간 복잡도 검증
✅ 메모리 사용량 체크
```

---

## 🚀 향후 계획

- [ ] Gold 문제 30개 돌파
- [ ] Platinum 도전
- [ ] 알고리즘 블로그 정리
- [ ] 코딩 테스트 대비 문제집 작성
- [ ] JavaScript 알고리즘 추가
- [ ] 자료구조 직접 구현 (Stack, Queue, Tree 등)

---

## 🤝 기여하기

이 레포는 개인 학습 기록이지만, 피드백은 언제나 환영합니다! 

### 기여 방법

1. Fork 이 저장소
2. 개선 사항 작성
3. Pull Request 생성

**피드백 환영:**
- 더 나은 풀이 방법
- 코드 최적화
- 오류 수정

---

## 📜 라이선스

이 프로젝트는 MIT License 하에 배포됩니다.

---

## 📞 연락처

<div align="center">

### 프로젝트 관리자:   Deamonio

[![Email](https://img.shields.io/badge/Email-hyun0810d@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hyun0810d@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Deamonio-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Deamonio)

**프로젝트 링크**:  [https://github.com/Deamonio/Algorithm-Workspace](https://github.com/Deamonio/Algorithm-Workspace)

</div>

---

## 🙏 감사의 말

| Jungol | Baekjoon | Programmers |
|---|---|---|
| 기초 문제 | 다양한 난이도 | 실전 대비 |

**특별 감사:**
- 🏫 **알고리즘 스터디원** - 함께 성장한 동료들
- 💻 **오픈소스 커뮤니티** - 풀이 참고 및 학습
- 📚 **문제 출제자** - 양질의 문제 제공

---

<div align="center">

## ⭐ 이 레포가 도움이 되셨다면 Star를 눌러주세요!  

[![Star History Chart](https://api.star-history.com/svg?repos=Deamonio/Algorithm-Workspace&type=Date)](https://star-history.com/#Deamonio/Algorithm-Workspace&Date)

---

**Made with 💻 by Deamonio**

*"매일 한 문제씩, 꾸준함이 실력이 된다"*

---

**© 2025 Deamonio.   All rights reserved.**

[⬆ 맨 위로 돌아가기](#-algorithm-workspace)

</div>
