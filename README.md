# 2021 오픈소스 컨트리뷰션 아카데미 - Tidyverse 데이터 과학
<img src = "https://www.tidyverse.org/images/tidyverse-default.png" width="12%" height="12%"> [Tidyverse 데이터 과학 소개](https://drive.google.com/file/d/1AFbgEz_hTackz9wzVgfKZ50CKZCtuCXs/view?usp=sharing)

## 1. 협업을 위한 기본 지식

[![오픈소스 참여를 위한 Git/GitHub 기본](https://img.shields.io/badge/-%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4%20%EC%B0%B8%EC%97%AC%EB%A5%BC%20%EC%9C%84%ED%95%9C%20Git/GitHub%20%EA%B8%B0%EB%B3%B8-black?style=flat-square&logo=git&logoColor=white)](https://drive.google.com/file/d/1vX3fTJf1yevDPGGrl-E6ANKjKnTz_Czu/view?usp=sharing)
[![오픈소스 참여를 위한 Git/GitHub 고급](https://img.shields.io/badge/-%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4%20%EC%B0%B8%EC%97%AC%EB%A5%BC%20%EC%9C%84%ED%95%9C%20Git/GitHub%20%EA%B3%A0%EA%B8%89-black?style=flat-square&logo=github&logoColor=white)](https://drive.google.com/file/d/1eo6LfqoXRVZmklNWleJcMfEJVl9zQpUr/view?usp=sharing)

### 1) Git/Github in Git Bash

```r
# fork한 repo 가져오기
git clone https://github.com/HwayoungYoon/pkg_doc.git
# 상태 확인
git status
# 전체 내용 선택
git add .
# commit message 입력
git commit -m "상세내용"
# push할 저장소 설정
git remote set-url origin https://github.com/HwayoungYoon/pkg_doc.git
# 저장소로 push
git push
git push --set-upstream origin master
```

### 2) 패키지 개발 in R

```r
# 패키지가 잘 작동하는지 확인
ctrl+shift+B : 팩키지 build
```

## 2. 온보딩

- 온보딩 페이지

[Open UP On-Boarding: 한국 통계 팩키지](https://r2bit.com/onboard/tong.html)

- OJT 튜토리얼 페이지

[Open UP On-Boarding: 오픈 통계 팩키지 OJT](https://r2bit.com/onboard/ojt.html)

## 3. R 패키지

### 1) 데이터 패키지(statdata)

[R 팩키지](https://statkclee.github.io/pkg/pkg-openstat-dataset.html)

통계 분석에 활용할 수 있는 데이터를 패키지로 만드는 작업.

### 2) 통계 패키지 문서

[GitHub - tidyverse-korea/pkg_doc: 통계팩키지 문서](https://github.com/tidyverse-korea/pkg_doc)

```r
# Rstudio에서 pkg_doc 실행
Open Project 클릭
pkg_doc.Rproj 실행
```

```r
# pkg_doc의 폴더 및 파일 설명
_site.yml : 사이트의 큰 틀
data 폴더 : 다운받은 데이터 저장
~~.Rmd : 각각의 html 페이지
```

```r
# 새로운 변수 형태 생성
# 단변량/이변량/다변량 & 범주형/연속형
_site.yml 파일 수정
"""      - text: "단변량 연속형 변수" """
"""        href: univariate-continuous.html """
~~.Rmd 파일 생성&수정 (More - copy - 이름 변경)
""" 이름을 univariate-continuous로 변경 """
생성한 ~~.Rmd 파일 수정
""" 데이터 파일, 설명 등 변경 """
```

- TO-DO : `gt` 패키지([Grammer of Tables](https://themockup.blog/posts/2020-05-16-gt-a-grammer-of-tables/))로 예쁘게 표를 만들 필요가 있음. (참고: [Grammer of Graphics](http://henryquant.blogspot.com/2019/09/grammar-of-graphics-ggplot.html))
- TO-DO : 행과 열을 전치하여 표를 제작하는 것도 필요함.

### 3) 오픈 통계 패키기(open_stat)

[GitHub - tidyverse-korea/open_stat: 오픈 통계 팩키지](https://github.com/tidyverse-korea/open_stat)

### 4) kodlookr 패키지

[kodlookr 패키지 개발하기](https://choonghyunryu.github.io/about_package/?fbclid=IwAR2lqzqHGIwsJcMR3sJ1I21nIqeZ4VdHRzw5yfcSsfVkJmIHyDg3giY-6QQ#1)
