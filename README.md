# Chapter1  
## 팀원 github hompage  
+ 강다빈  
  + [강다빈 깃 허브 사이트](https://dabin0513.github.io/)  
  
# Chapter2  
## 컴퓨터 데이터 구조(강다빈)    
# Stack  
>+ FILO: First In Last Out  
>+ push: 새로운 요소 추가  
>+ pop: 가장 최근에 들어오는 것을 지우기    
>+ Stack의 활용 예시  
>  + 후위 표기법 계산  
>  + 수식의 괄호 검사(연산자 우선순위 표현을 위한 괄호 검사)  

![Stack 사진](https://user-images.githubusercontent.com/63287630/86358634-c5f74400-bcaa-11ea-9082-b3984a33a06e.png)  
+ Stack은 데이터의 삽입과 삭제가 한 방향에서만 이루어지는데 삽입과 삭제가 일어나는 위치를 top이라고 합니다.  

# Queue  
>+ FIFO: First In First Out  
>+ Enqueue: 가장 늦게 온 것은 가장 뒤에  
>+ Dequeue: 가장 앞에 있는 것을 가장 먼저 삭제  
>+ Queue의 활용 예시  
>  + 은행 업무  
>  + 콜센터 고객 대기시간  
>  + 프로세스 관리  
>  + 너비 우선 탐색(BFS, Breath-First Search)구현  

![Queue 사진](https://user-images.githubusercontent.com/63287630/86358684-ddcec800-bcaa-11ea-85fb-1e210287c388.png)  
+ 출구를 머리(front)로 정해서 삭제를 수행하고, 입구는 꼬리(rear)로 정해서 삽입을 수행합니다.  
 
# 트리(Tree)
> + 트리는 노드로 이루어진 자료 구조를 말합니다.
>   + 트리는 하나의 루트 노드를 가집니다.
>   + 루트 노드는 0개 이상의 자식 노드를 갖고 있습니다.
>   + 그 자식 노드 또한 0개 이상의 자식노드를 가지고 있고, 이는 반복적으로 정의 됩니다.

![트리](https://user-images.githubusercontent.com/63287630/86360770-d0670d00-bcad-11ea-928b-012c456acd72.png)

# 트리와 관련된 용어
>      + 루트 노드(root node): 부모가 없는 노드로 트리는 하나의 루트 노드만을 가짐
>      + 단말 노드(leaf node): 자식이 없는 노드를 말합니다.
>      + 내부 노드(internal node): 단말노드가 아닌 노드
>      + 간선(edge): 노드를 연결하는 선
>      + 형제(sibling): 같은 부모를 가진 노드
>      + 노드의 사이즈(size): 자신을 포함한 모든 자손 노드의 개수
>      + 노드의 깊이(depth): 루트에서 어떤 노드에 도달하기 위해 거쳐야 하는 간선의 수
>      + 노드의 레벨(level): 트리의 특정 깊이를 가지는 노드의 집합
>      + 노드의 차수(degree): 하위 트리 개수/ 간선수(degree): 각 노드가 지닌 가지의 수
>      + 트리의 차수(degree of tree): 트리의 최대 차수
>      + 트리의 높이(height): 루트 노드에서 가장 깊숙히 있는 노드의 깊이




## 프로그래밍 응용 1
#### 자바란?

1. 완전한 객체지향 언어이며, 객체지향의 특성인 클래스, 상속, 캡슐화, 다형성 등의 개념이 적  용된 언어이다.  

#### 조건문  
- switch-case문
```java
switch(조건식){
	case: 조건1
    	break;
    case: 조건2
    	break;
    default:
```  

- if 문  
```java
if(조건삭){//조건식이 true일 때 아래 실행문 동작
	실행문;
    실행문;
 }
```  

#### 반복문  
- while문 
```java
while(조건식){}
```

- do-while문 
```java
 do {} while(조건식);
```

- for문 
```java
for(초기식; 조건식; 증감식){}
```
