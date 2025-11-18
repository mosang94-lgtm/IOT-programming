오늘 주제  : 1.if 조건식 2. if/else 조건식 3. if/elif 조건식

1)배송비

price = int(input("상품의 가격 : "))
if price  > 20000:
shippingCost = 0
print("VIP 고객님", end="")
else:
shippingCost = 3000
print("고객님", end="")
print(f"배송비는 {shippingCost} 입니다.")

2)윤년

year = int(input("년도 입력 : "))`
if year %4==0 and year % 100 != 0 or year %400 ==0:
print(f"{year}년은 윤년(leap year)입니다.")
else:    print(f"{year}년은 평년(common year)입니다.")

연산자 우선순위가 다 정해져 있다(공부하기)

3)
import  randomo = random.randint(1,2)
x= random.randint(1,100)
y= random.randint(1,100)
if op == 1:
answer = int(input(f"{x} + {y} ="))
if answer == x+y:
print("정답입니다.")
else: print("틀렸습니다.")else:    answer = int(input(f"{x} + {y} ="))    if answer == x-y:        print("정답입니다.")    else:        print("틀렸습니다.")`

#점수를 입력받아 등급을 출력하는 프로그램을 작성하시오.
#90점이상 A, 80점 이상 B, 70점 이상 C, 60점 이상 D, 60점 미만은 F
score=int(input("점수 입력 : "))
if score >=90: 
grade="A"
elif score >=80:
grade="B"
elif score >=70:  
grade="C"
elif score >=60:
grade="D"
else:   
grade="F"
print(f"점수는 {score}이고 등급은 {grade} 입니다.")`
--------------
for 구문 예시
evenSum = 0
oddSum = 0
sevenSum = 0

for i in range(101):
    if i % 2 == 0:
        evenSum += i
    else:
        oddSum += i
    if i % 7==0:
        sevenSum += i


print(f"1부터 100까지의 홀수들의 합은  {oddSum} 입니다.")
print(f"1부터 100까지의 짝수들의 합은  {evenSum} 입니다.")
print(f"1부터 100까지의 7의 배수들의 합은  {sevenSum} 입니다.")

