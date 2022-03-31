# 쉘 스크립트 for문

### 기본 문법
```
# 1. for ()
for ((초기값;조건식;증감));do
  ~
done

# 2. for in
for 변수 in 값
do
  ~
done
```
1. for ()<br>
일반적인 코딩문법과 동일하다. 대신 이중 괄호를 사용해야 하며, 조건식 뒤에 ```;do```를(줄바꿈시에는 do만) 작성한 이후에 수행문을 작성해야 하며 마무리는 ```done```로 끝나야 한다.<br><br>
2. for in<br>
다른 언어의 foreach, for in, for of 형태이며 리스트나 배열의 모든 원소들에 접근하는 형태이다.<br>
조건식만 제외하고는 for ()문법과 동일하다.

---

### 응용 예제
```
# 1. 값 띄어쓰기
for var in A B C;do ~; done

# 2. 리스트
list="A B C"
for var in ${list};do ~; done

# 3. 배열
arr=("A" "B" "C")
for var in ${arr[@]};do ~; done

# 4. 순차 증가
for var in {1..100};do ~; done

# 5. 순차 증가(증감폭)
for var in {1..100..5};do ~; done
```
