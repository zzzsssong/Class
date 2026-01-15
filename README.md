# Class
# 🐍 파이썬 기초 퀴즈

앞서 학습한 5개의 샘플 코드를 기반으로 한 퀴즈입니다. 각 문제를 풀어보고 정답을 확인하세요!

---

## 퀴즈 1: 변수와 데이터 타입

**다음 코드의 출력 결과는?**

```python
name = '파이썬'
version = 3.12
print(type(name), type(version))
```

**선택지:**
1. `<class 'str'> <class 'int'>`
2. `<class 'str'> <class 'float'>`
3. `<class 'string'> <class 'float'>`
4. `<class 'text'> <class 'number'>`

<details>
<summary>정답 보기</summary>

**정답: 2번**

`name`은 문자열(str), `version`은 실수(float)입니다. 3.12는 소수점이 있어 float 타입입니다.

</details>

---

## 퀴즈 2: 리스트 인덱싱

**다음 코드의 출력 결과는?**

```python
fruits = ['사과', '바나나', '오렌지', '포도']
print(fruits[-2])
```

**선택지:**
1. 바나나
2. 오렌지
3. 포도
4. 에러 발생

<details>
<summary>정답 보기</summary>

**정답: 2번 (오렌지)**

음수 인덱스는 뒤에서부터 세며, `-1`이 마지막, `-2`가 뒤에서 두 번째입니다.

</details>

---

## 퀴즈 3: 조건문

**다음 코드의 출력 결과는?**

```python
score = 85
if score >= 90:
    print('A')
elif score >= 80:
    print('B')
else:
    print('C')
```

**선택지:**
1. A
2. B
3. C
4. 아무것도 출력 안됨

<details>
<summary>정답 보기</summary>

**정답: 2번 (B)**

`score`는 85이므로 두 번째 조건(`>= 80`)을 만족하여 'B'가 출력됩니다.

</details>

---

## 퀴즈 4: for 반복문

**다음 코드의 출력 결과는?**

```python
total = 0
for i in range(1, 5):
    total += i
print(total)
```

**선택지:**
1. 10
2. 15
3. 5
4. 0

<details>
<summary>정답 보기</summary>

**정답: 1번 (10)**

`range(1, 5)`는 1, 2, 3, 4를 생성하고, 합은 1+2+3+4 = 10입니다.

</details>

---

## 퀴즈 5: 함수 반환값

**다음 코드의 출력 결과는?**

```python
def multiply(a, b):
    return a * b

result = multiply(3, 4)
print(result)
```

**선택지:**
1. 7
2. 12
3. 34
4. None

<details>
<summary>정답 보기</summary>

**정답: 2번 (12)**

`multiply` 함수는 두 수를 곱한 값을 반환합니다. 3 × 4 = 12입니다.

</details>

---

## 퀴즈 6: 리스트 메서드

**다음 코드 실행 후 `numbers`의 값은?**

```python
numbers = [1, 2, 3]
numbers.append(4)
numbers.insert(0, 0)
print(numbers)
```

**선택지:**
1. `[1, 2, 3, 4, 0]`
2. `[0, 1, 2, 3, 4]`
3. `[1, 2, 3, 4]`
4. `[0, 1, 2, 3]`

<details>
<summary>정답 보기</summary>

**정답: 2번 (`[0, 1, 2, 3, 4]`)**

`append(4)`로 끝에 4를 추가하고, `insert(0, 0)`으로 맨 앞(인덱스 0)에 0을 삽입합니다.

</details>

---

## 퀴즈 7: 딕셔너리

**다음 코드의 출력 결과는?**

```python
student = {'이름': '김철수', '나이': 20}
print(student['이름'])
```

**선택지:**
1. 김철수
2. '김철수'
3. 이름
4. 에러 발생

<details>
<summary>정답 보기</summary>

**정답: 1번 (김철수)**

딕셔너리에서 키로 값을 조회하면 해당 값이 출력됩니다. `student['이름']`은 키 '이름'에 해당하는 값 '김철수'를 반환합니다.

</details>

---

## 퀴즈 8: while 반복문과 break

**다음 코드의 출력 결과는?**

```python
count = 0
while True:
    count += 1
    if count == 3:
        break
print(count)
```

**선택지:**
1. 1
2. 2
3. 3
4. 무한 루프

<details>
<summary>정답 보기</summary>

**정답: 3번 (3)**

`count`가 3이 되는 순간 `break`가 실행되어 반복문을 종료하고 3이 출력됩니다.

</details>

---

## 퀴즈 9: 리스트 슬라이싱

**다음 코드의 출력 결과는?**

```python
numbers = [10, 20, 30, 40, 50]
print(numbers[1:4])
```

**선택지:**
1. `[10, 20, 30]`
2. `[20, 30, 40]`
3. `[20, 30, 40, 50]`
4. `[10, 20, 30, 40]`

<details>
<summary>정답 보기</summary>

**정답: 2번 (`[20, 30, 40]`)**

슬라이싱 `[1:4]`는 인덱스 1부터 3까지(4는 미포함)를 의미합니다. 인덱스 1, 2, 3의 항목을 포함합니다.

</details>

---

## 퀴즈 10: 함수 기본 매개변수

**다음 코드의 출력 결과는?**

```python
def greet(name, msg='안녕하세요'):
    return f'{msg}, {name}님!'

print(greet('홍길동'))
```

**선택지:**
1. 안녕하세요, 홍길동님!
2. 홍길동님!
3. 안녕하세요
4. 에러 발생

<details>
<summary>정답 보기</summary>

**정답: 1번 (안녕하세요, 홍길동님!)**

`msg` 매개변수에 값을 전달하지 않으면 기본값 '안녕하세요'가 사용됩니다.

</details>

---

## 📊 점수 계산

정답 개수를 세어보세요!

- **10개**: 🏆 완벽합니다! 파이썬 기초를 완전히 마스터했습니다!
- **8-9개**: 🌟 훌륭합니다! 파이썬 기초를 잘 이해하고 있습니다!
- **6-7개**: 👍 좋습니다! 조금만 더 복습하면 완벽해질 거예요!
- **4-5개**: 📚 괜찮습니다! 샘플 코드를 다시 한 번 복습해보세요!
- **0-3개**: 💪 화이팅! 샘플 코드를 천천히 다시 학습해보세요!

## 📚 복습 자료

틀린 문제가 있다면 해당 샘플 코드를 다시 확인해보세요:

- [01_variables_and_data_types.py](file:///c:/Users/USER/Desktop/01_variables_and_data_types.py) - 변수와 데이터 타입
- [02_conditional_statements.py](file:///c:/Users/USER/Desktop/02_conditional_statements.py) - 조건문
- [03_loops.py](file:///c:/Users/USER/Desktop/03_loops.py) - 반복문
- [04_functions.py](file:///c:/Users/USER/Desktop/04_functions.py) - 함수
- [05_list_operations.py](file:///c:/Users/USER/Desktop/05_list_operations.py) - 리스트 조작

