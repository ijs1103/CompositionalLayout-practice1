# CompositionalLayout-practice1

![Simulator Screen Recording - iPhone 13 Pro - 2023-01-12 at 23 38 47](https://user-images.githubusercontent.com/42196410/212100513-364e264b-d77a-40f9-b037-da82c025f65a.gif)


## 🧩 개요

- `CompositionalLayout`로 동적인 높이의 Item을 가지는 리스트를 화면에 표현. 

- 버튼 클릭시 다른 데이터를 가지는 리스트를 표현.

## 🤔 배운 내용

### ✔️ CompositionalLayout

기존의 `UICollectionView`에서 복잡한 layout을 구현할 때 상당한 난이도가 요구되는데 `CompositionalLayout`로 보다 쉽게 구현할 수 있다.

### ✔️ UICollectionViewDiffableDataSource

기존의 `UICollectionViewDataSource`에서 복잡한 layout을 구현할 때 `Controller와 UI의 데이터가 일치하지 않는 문제`가 발생할 수 있다.

따라서, 이러한 문제를 해결하기 위해 `Single Source of Truth`를 가능케하는 `Snapshot`객체로 하나의 데이터만을 관리하게 한다.

`Snapshot`은 섹션 및 아이템에 대해 기존의 IndexPath를 사용하지 않고, UID를 사용한다.

### ✔️ 아이템의 동적 높이 설정

`heightDimension`값을 `.estimated` 메서드로 설정한다
