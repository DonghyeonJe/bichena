비채나는 비우고 채우고 나누다 라는 뜻입니다.

MZ세대를 목표로한 트렌디한 전통주 판매 사이트 

![screencapture-bichena-kro-kr-main-ko-2024-05-24-09_36_12 (1).png](https://prod-files-secure.s3.us-west-2.amazonaws.com/44404258-d2d4-4daf-86cf-6ae797e7bc03/b66410a2-daf7-47ce-96c9-51c725b3e426/69848f0b-14f0-4515-9a5b-09c73f7921b1.png)

**요약**

- MZ세대를 겨냥한 트렌디한 전통주 판매 사이트 기획 및 제작
- 비우고 채우고 나누다 라는 뜻의 비채나

**담당한 역할** 

- 총 7명 이 함께 진행
- 프로젝트 부총괄
- 홈페이지 디자인 전반 총괄 (Figma)
- 홈페이지/관리자 페이지 NAVBAR
- 메인 페이지
- 상품 리스트 페이지
- 담당부분 반응형 처리
- Google chartAPI를 이용한 차트 구현(관리자 페이지)

**개발환경**

- FrameWork : SpringFramework , MyBatis , Bootstrap3,4
- 서버&DB : Apache Tomcat, MariaDB
- 언어 : HTML , JS , CSS ,
- 라이브러리 : jQuery , Jstl
- 클라우드 서비스 : AWS

**시기**

- 2024.04 ~ 2024.05

# 📝 전통주 판매 사이트 제작 및 상품 등록

---

- 홈페이지 : http://bichena.kro.kr/main.ko

- GitHub

https://github.com/DonghyeonJe/Bichena.git

- 작업한 내용

![screencapture-bichena-kro-kr-main-ko-2024-07-01-13_19_51.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/44404258-d2d4-4daf-86cf-6ae797e7bc03/9d5eff29-34df-4de9-b6a7-749479d8dc5d/screencapture-bichena-kro-kr-main-ko-2024-07-01-13_19_51.png)

- swiper와 slick  두 종류의 슬라이드를 총 6개 사용해서 메인화면을 구성하였습니다.
- MyBatis의 Mapper를 이용해서 DB내의 술종류 컬럼에 해당하는 데이터를 가져와 각 슬라이더마다  종류 별로 출력되게 만들었습니다.
- DB내의 상품 테이블의 상품이름,상품설명,상품가격,단맛,신맛,탄산,도수, 상품이미지 항목을 불러왔습니다.
- 베스트 리뷰 슬라이드는 prodrev테이블의 유저닉네임,평점,상품이미지,리뷰내용의 컬럼 내용을 최신글에서 불러와서 출력했습니다.

![screencapture-bichena-kro-kr-prodList-ko-2024-06-26-12_31_58.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/44404258-d2d4-4daf-86cf-6ae797e7bc03/47ebdc08-a2d8-4558-b14c-861f120a7ef7/screencapture-bichena-kro-kr-prodList-ko-2024-06-26-12_31_58.png)

- grid를 이용하여 한 화면에 16개의 상품을 정렬하여 불러오도록 구현하였습니다.
- 필터를 이용하여 주종,단맛,신맛,탄산,원료에 해당하는 상품을 불러오도록 구현하였습니다.
- pagination 기능을 이용하여 불러온 상품의 갯수가 16개를 넘으면 페이징 처리되게 하였습니다.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/44404258-d2d4-4daf-86cf-6ae797e7bc03/88b83aaf-d710-48b8-b177-acb6be8ade66/Untitled.png)

- 관리자 페이지에서 판매현황 부분입니다.
- Google Chart API를 이용해서 모든 상품들의 판매 순위중 내림차순 정렬로 제일 많이 판매된 갯수를 상위에서부터 5개 표시하였습니다.
- 갯수를 출력할때 총 판매 물량에서 주문취소 된 물량을 빼고 출력되게 하였습니다.
