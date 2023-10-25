## Priority queue

큐와 유사하지만 우선순위가 높은 아이템이 먼저 처리됨

### 우선순위 큐 주요 동작

- insert: 큐에 아이템을 넣음. 아이템의 우선순위 정보도 같이 넣어줌
- delete: 가장 우선순위가 높은 아이템을 빼내는 것
- peek: delete와 같지만 우선순위 큐에서 제거하지 않음

### 우선순위 큐 동작 방식 설명

## Heap

- 힙은 주로 이진 트리(binary tree) 기반으로 구현
- max heap과 min heap이 있음

>[!NOTE]
>**트리(tree)**
>
>부모-자녀처럼 계층적인 형태를 가지는 구조
>
>**이진 트리(binary tree)**
>
>자녀가 최대 두 개인 트리

### max heap

max heap 예시 그림

부모 노드의 키(key)가 자식 노드(들)의 키(key)보다 크거나 같은 트리

그림에 있는 것처럼 트리에 있는 모든 부모 노드들이 자기 자녀들의 키값보다 같거나 클 때 max heap이라고 함

### min heap

부모 노드의 키(key)가 자식 노드(들)의 키(key)보다 작거나 같은 트리

max heap의 반대로 생각하면 이해할 수 있음

### 힙 주요 동작

- insert: 힙에 아이템의 키값을 같이 넣어줌
- delete: max heap이라면 키값이 가장 큰 아이템을 반환하고, min heap이라면 키값이 가장 작은 아이템을 반환함
- peek: delete와 같지만 힙에서 제거하지 않음

### max heap: insert(17)

예시 그림

max heap에서 insert(17)을 했을 때 동작하는 방식

### max heap: delete()

예시 그림

max heap에서 delete가 동작하는 방식
가장 최상단에 있는 노드를 root node라고 하는데, max heap에서는 root node의 키값이 전체트리에서 가장 크다. 
그렇기 때문에 delete()를 호출하게 되면 max heap에서 가장 큰 아이템을 꺼낸다. 그러면 root node가 비워지는데 이때 가장 끝에있는 노드를 넣어준다.
그러고나서 자식 노드의 키값보다 크면 위치를 재조정해준다.

## Priority queue와 Heap의 관계


