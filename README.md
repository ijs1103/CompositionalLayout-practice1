# CompositionalLayout-practice1

![Simulator Screen Recording - iPhone 13 Pro - 2023-01-12 at 23 38 47](https://user-images.githubusercontent.com/42196410/212100513-364e264b-d77a-40f9-b037-da82c025f65a.gif)


## ๐งฉ ๊ฐ์

- `CompositionalLayout`๋ก ๋์ ์ธ ๋์ด์ Item์ ๊ฐ์ง๋ ๋ฆฌ์คํธ๋ฅผ ํ๋ฉด์ ํํ. 

- ๋ฒํผ ํด๋ฆญ์ ๋ค๋ฅธ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ง๋ ๋ฆฌ์คํธ๋ฅผ ํํ.

## ๐ค ๋ฐฐ์ด ๋ด์ฉ

### โ๏ธ CompositionalLayout

๊ธฐ์กด์ `UICollectionView`์์ ๋ณต์กํ layout์ ๊ตฌํํ  ๋ ์๋นํ ๋์ด๋๊ฐ ์๊ตฌ๋๋๋ฐ `CompositionalLayout`๋ก ๋ณด๋ค ์ฝ๊ฒ ๊ตฌํํ  ์ ์๋ค.

### โ๏ธ UICollectionViewDiffableDataSource

๊ธฐ์กด์ `UICollectionViewDataSource`์์ ๋ณต์กํ layout์ ๊ตฌํํ  ๋ `Controller์ UI์ ๋ฐ์ดํฐ๊ฐ ์ผ์นํ์ง ์๋ ๋ฌธ์ `๊ฐ ๋ฐ์ํ  ์ ์๋ค.

๋ฐ๋ผ์, ์ด๋ฌํ ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด `Single Source of Truth`๋ฅผ ๊ฐ๋ฅ์ผํ๋ `Snapshot`๊ฐ์ฒด๋ก ํ๋์ ๋ฐ์ดํฐ๋ง์ ๊ด๋ฆฌํ๊ฒ ํ๋ค.

`Snapshot`์ ์น์ ๋ฐ ์์ดํ์ ๋ํด ๊ธฐ์กด์ IndexPath๋ฅผ ์ฌ์ฉํ์ง ์๊ณ , UID๋ฅผ ์ฌ์ฉํ๋ค.

### โ๏ธ ์์ดํ์ ๋์  ๋์ด ์ค์ 

`heightDimension`๊ฐ์ `.estimated` ๋ฉ์๋๋ก ์ค์ ํ๋ค
